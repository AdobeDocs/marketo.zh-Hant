---
description: Dynamic Chat 發行說明 - Marketo 文件 - 產品文件
title: Dynamic Chat 發行說明
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '3408'
ht-degree: 1%

---

# Dynamic Chat 發行說明 {#dynamic-chat-release}

Adobe Dynamic Chat版本會在持續傳遞模式上運作，允許以更可擴充的方法進行功能部署。 有時候一個月會有多個版本，所以請定期回來檢視最新的資訊。

您可在此處[找到Marketo Engage ](/help/marketo/release-notes/current.md){target="_blank"}的標準發行說明頁面。

## 2025 年 6 月發行版本 {#june-2025-release}

**發行日期： 2025年6月30日**

### 路由邏輯改寫 {#routing-logic-revamp}

我們已改寫Dynamic Chat中的即時聊天路由邏輯，以確保所有路由型別（帳戶、自訂、團隊和循環配置資源）都有更智慧型且可預測的參與行為。 新的邏輯簡化了路由流程，並改善了代理程式無法使用時的遞補處理。

#### 路由行為的重要改善

* **每個工作階段最多兩次參與嘗試**

   * 系統將嘗試連線最多兩個代理程式（最多），但必須嚴格遵循主要路由規則。

   * 如果代理程式可用但未回應（例如，拒絕或遺漏聊天），系統會嘗試從相同集區連線到不同的代理程式。

   * 只有在初始解析期間找不到符合資格的代理程式時，才會啟用遞補邏輯（例如循環配置資源），而不是在失敗的參與之後重試。

* **路由規則特定行為**

##### — 帳戶路由 — 

如果訪客的電子郵件網域對應到已知帳戶，則永遠會優先處理對應的代理程式。

如果代理程式可用，則會直接將聊天路由給他們。

如果代理程式無法使用，則系統：

* 不嘗試其他代理程式，即使啟用遞回配置資源作為遞補也是如此。

* 相反地，它：

   * 顯示對應代理程式的會議行事曆（如果啟用），
 — 或 — 
   * 回覆為預設訊息（最壞的情況）。

只有當帳戶路由不符合資格（沒有相符的網域或代理程式）時，才會考慮卡片層級路由規則（例如，團隊、自訂）。

##### — 自訂/團隊路由 — 

這些規則可能會傳回多個符合資格的代理程式。

如果第一個可用的代理程式未參與，系統會從相同清單中再嘗試一個代理程式。

因為有一個代理程式沒有回應，所以不會觸發循環配置資源遞補機制。

如果兩個代理程式都未參與：

* 系統會顯示第一個嘗試代理程式的行事曆（如果已啟用），
 — 或 — 
* 顯示預設的遞補訊息。

##### — 循環配置資源路由 — 

當作為主要路由規則使用時，系統：

* 嘗試從循環配置資源集區中接洽第一個可用的代理程式。

* 如果第一個代理程式沒有回應，它會以下一個最佳合格代理程式重試。

如果將「循環配置資源」用作遞補資源，則只有在未從主要規則解析任何代理程式時，它才會啟動。

##### 訪客體驗流程

系統會檢查「帳戶路由」是否適用。

* 如果是，而且代理程式可用，就會立即連線。

* 如果代理程式不符合資格或無法使用，則會繼續進行卡片層級的路由規則。

會評估卡片層級路由規則（自訂、團隊、循環配置資源）。

* 系統會檢查合格代理程式的可用性（許可權、狀態）。

* 系統會啟動一個代理程式，並在必要時嘗試使用相同規則的第二個代理程式。

* 如果沒有參與成功，則會套用遞補邏輯：

   * 日曆遞補（若已啟用）、
 — 或 — 
   * 預設訊息。

只有在主要路由規則中找不到符合資格的代理程式時，才會考量循環配置資源遞補機制，而不是在個別代理程式無法回應時。

##### 使用案例

<p>

_&#x200B;**帳戶路由**&#x200B;_

<table><thead>
  <tr>
    <th>類型</th>
    <th>範例</th>
    <th>結果</th>
  </tr></thead>
<tbody>
  <tr>
    <td>理想</td>
    <td>訪客的網域對應到帳戶；對應的代理程式已啟用即時聊天並可供使用</td>
    <td>聊天直接連線到對應的代理程式</td>
  </tr>
  <tr>
    <td>遞補（循環配置資源）</td>
    <td>無法使用對應的代理程式，已啟用循環配置資源遞補</td>
    <td>系統透過Round Robin選取一個可用的代理程式並讓他們參與 </td>
  </tr>
  <tr>
    <td>沒有遞補代理程式</td>
    <td>對應的代理程式無法使用，沒有循環配置資源遞補機制；會議預約已啟用</td>
    <td>系統會顯示對應代理程式的行事曆或顯示預設的遞補訊息</td>
  </tr>
</tbody></table>

_&#x200B;**自訂路由**&#x200B;_

<table><thead>
  <tr>
    <th>類型</th>
    <th>範例</th>
    <th>結果</th>
  </tr></thead>
<tbody>
  <tr>
    <td>理想</td>
    <td>自訂邏輯會解析代理程式清單；第一個代理程式可用並接受聊天。</td>
    <td>聊天連線到第一個代理程式。</td>
  </tr>
  <tr>
    <td>遞補（循環配置資源）</td>
    <td>自訂規則未解析任何代理程式，已啟用循環配置資源遞補。</td>
    <td>系統透過Round Robin選取一個可用的代理程式並啟動它們。</td>
  </tr>
  <tr>
    <td>沒有遞補代理程式</td>
    <td>兩個代理程式已解決；兩個代理程式都不接受聊天，後援設定為會議行事曆。</td>
    <td>顯示第一次嘗試代理程式的行事曆或顯示預設的遞補訊息。</td>
  </tr>
</tbody></table>

_&#x200B;**團隊路由**&#x200B;_

<table><thead>
  <tr>
    <th>類型</th>
    <th>範例</th>
    <th>結果</th>
  </tr></thead>
<tbody>
  <tr>
    <td>理想</td>
    <td>團隊包括擁有即時聊天內容的代理程式；第一個可用的代理程式接受聊天。</td>
    <td>聊天連線至該代理程式。</td>
  </tr>
  <tr>
    <td>遞補（循環配置資源）</td>
    <td>沒有可用的群組代理程式，且已啟用循環配置資源遞補功能。</td>
    <td>系統從Round Robin集區選取一個代理程式並連線。</td>
  </tr>
  <tr>
    <td>沒有遞補代理程式</td>
    <td>有兩個代理程式可供使用，但兩者皆不參與；已啟用行事曆遞補。</td>
    <td>顯示首次嘗試代理程式的行事曆或觸發遞補訊息。</td>
  </tr>
</tbody></table>

_&#x200B;**循環配置資源路由**&#x200B;_

<table><thead>
  <tr>
    <th>類型</th>
    <th>範例</th>
    <th>結果</th>
  </tr></thead>
<tbody>
  <tr>
    <td>理想</td>
    <td>Round Robin集區有多個代理程式；第二個代理程式接受第一個不接受之後的聊天。</td>
    <td>聊天連線到第二個代理程式。</td>
  </tr>
  <tr>
    <td>遞補（循環配置資源）</td>
    <td>Round Robin集區中沒有可用的代理程式；已啟用會議行事曆。</td>
    <td>行事曆會針對清單中的第一個代理程式顯示（若已設定），或顯示遞補訊息。</td>
  </tr>
  <tr>
    <td>沒有遞補代理程式</td>
    <td>沒有可用的代理程式；已停用遞補。</td>
    <td>靜態後援訊息會向訪客顯示。</td>
  </tr>
</tbody></table>

### Pulse通知 {#pulse-notification}

每當訪客請求與代理程式連線時，我們都會向代理程式提供應用程式內瀏覽器通知。 但有時，代理會忽略這些聊天。

在此版本中，當新訪客有興趣聊天時，即時代理程式會收到電子郵件、Slack、應用程式內和瀏覽器通知。

1. 在您的Adobe Experience Cloud首頁上，按一下「帳戶」圖示並選取&#x200B;**偏好設定**。

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. 向下捲動至&#x200B;_通知_，並選取所需的Dynamic Chat。

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Pulse通知的內容可與我們用於應用程式內瀏覽器通知的內容相同。

## 2025年4/5月發行版本 {#apr-may-25-release}

### 訊息通知音效 {#message-notification-sound}

您現在可以選擇在工作階段中每次觸發聊天機器人時都為訪客啟用音效。 有多種聲音可供選擇。

### 在行動裝置上啟用Poke訊息 {#enable-poke-messages-on-mobile}

「撥號」會顯示在聊天圖示旁的開頭問題，訪客不需要按一下即可檢視，現在為使用行動裝置的訪客啟用此選項。

### 預設遞補更新 {#default-fallback-update}

對於任何作為即時聊天卡的自訂規則/團隊 — 如果沒有可用的代理程式（或聊天無法連線），它會回退到可用代理程式的Round Robin （無論將哪個路由邏輯/規則放在資料流中，當時所有可用的代理程式）。

### Demandbase整合 {#demandbase-integration}

Demandbase使用者可以使用Demandbase人員屬性來進行Dynamic Chat中的對話方塊目標定位、條件式品牌和自訂路由。

## 2024年9/10月發行版本 {#sep-oct-release}

### 增強型即時聊天分析 {#enhanced-live-chat-analytics}

Analytics Dashboard已進行數個增強功能，包括：

* 請求的即時聊天總數：「與代理商聊天」請求的訪客數

* 連線的即時聊天總數：已連線的訪客數與「與代理商聊天」的請求總數

* 未接的即時聊天請求總數：「與代理聊天」的無人參與訪客數與請求總數

* 以分鐘為單位的平均聊天長度：分析訪客與您的代理之間的「平均聊天長度」

* 平均代理程式回應時間（秒）：分析代理程式回應其即時聊天問答的「平均所用時間」

* 每日儀表板：即時聊天請求已成功連線、即時聊天請求已錯過、排序和篩選最近的即時聊天活動

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### 交談評分 {#conversation-scoring}

根據聊天互動的品品質化您的銷售機會，並將該量度用作Marketo Engage Smart Campaigns中的觸發器/篩選器。 在下列活動中使用新屬性&#x200B;_交談分數_：

* 與對話方塊互動
* 已參與交談流程
* 與代理程式互動

**注意事項：**

* 分數值將來自0、1、2、3 （預設值為空值）

* 當交談完成或捨棄時，無法編輯評分值

* 設定分數：

   * 在代理程式收件匣中 — 在即時聊天期間，代理程式可以更新或設定對話的分數，該分數會儲存在對話活動中

   * 在資料流設計工具中 — 在目標卡片中，使用者可以更新或設定交談的分數

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### 新的潛在客戶建立邏輯 {#new-lead-creation-logic}

如果潛在客戶填入具有電子郵件`abc@test.com`的表單並以xyz編碼，稍後再填入具有電子郵件`def@test.com`的相同表單，則會建立新的人員記錄，但cookie xyz會與新的人員產生關聯並從人員`abc@test.com`中移除。

因此，當具有Cookie abc的訪客登陸頁面並提供電子郵件ID為`abc@test.com`時：

<table><thead>
  <tr>
    <th>Visitor</th>
    <th>Cookie</th>
    <th>已提供電子郵件</th>
    <th>預期行為</th>
  </tr></thead>
<tbody>
  <tr>
    <td>匿名</td>
    <td>abc</td>
    <td>資料庫中不存在</td>
    <td>建立新人員</td>
  </tr>
  <tr>
    <td>匿名</td>
    <td>abc</td>
    <td>存在於資料庫中</td>
    <td>合併人員</td>
  </tr>
  <tr>
    <td>匿名</td>
    <td>xyz</td>
    <td>存在於資料庫中</td>
    <td>合併人員</td>
  </tr>
  <tr>
    <td>已知人員</td>
    <td>abc</td>
    <td>與現有人員相同</td>
    <td>更新人員</td>
  </tr>
  <tr>
    <td>已知人員</td>
    <td>abc</td>
    <td>與現有人員不同</td>
    <td>如果已經有已知人員存在，則轉移Cookie並解析該設定檔。 如果此電子郵件中沒有人員，請建立新的人員記錄並轉移Cookie</td>
  </tr>
  <tr>
    <td>已知人員</td>
    <td>xyz</td>
    <td>與現有人員相同</td>
    <td>將新Cookie新增至同一個人</td>
  </tr>
  <tr>
    <td>已知人員</td>
    <td>xyz</td>
    <td>與現有人員不同</td>
    <td>這種情況不可能發生，就好像它是新的Cookie，來自   預設為新的匿名設定檔</td>
  </tr>
</tbody></table>

### 繼承字型的選項 {#option-to-inherit-font}

您現在可以啟用聊天機器人直接從託管它的網頁繼承字型，而不是在Dynamic Chat中管理品牌字型。 啟用此選項時，聊天機器人會採用頁面`<body>`標籤上定義的字型。

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Demandbase與Dynamic Chat整合 {#demandbase-integration-with-dynamic-chat}

Demandbase使用者能夠自攜Demandbase授權並啟用整合。 使用Demandbase人員屬性進行對話方塊目標定位、條件式品牌和自訂路由。

這些屬性值對個人的解決會即時完成，並儲存在各自的人員設定檔中。

### 最佳化的交談流程載入時間 {#optimized-conversation-flow-load-time}

為了改善使用者體驗，現在會在載入對話流程時顯示閃爍的載入器，而非空白區域。

**在**&#x200B;之前

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**After**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## 2024 年 8 月發行版本 {#august-release}

**發行日期： 2024年8月23日**

### 自訂您的交談訊息格式 {#custom-format-conversation-messages}

串流設計工具現在支援[插入HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"}，以自訂您交談的外觀與風格。

![](assets/dynamic-chat-aug-2024-release-1.png)

### 聊天機器人捲動至底部 {#chatbot-scroll-to-bottom}

聊天機器人已新增圖示，讓網頁訪客直接跳至最後一則訊息。 這有助於訪客捲動文字以快速回到交談。

![](assets/dynamic-chat-aug-2024-release-2.png)

### 核心脈衝通知 {#core-pulse-notifications}

使用者現在會在會議預約或即時聊天失敗時收到[電子郵件通知](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"}。

![](assets/dynamic-chat-aug-2024-release-3.png)

### 支援多個交談 {#support-for-multiple-conversations}

聊天機器人現在支援多個交談。 網站訪客可同時參與不同頁面上的不同交談，且可在這些對話之間切換。

![](assets/dynamic-chat-aug-2024-release-4.png)

### 內容的預設排序 {#default-sorting-for-content}

依照預設，您的交談記錄、未回答的問題和問題產生表會依建立日期（從最近到最舊）排序。

### 即時銷售機會解析 {#real-time-lead-resolution}

在與匿名潛在客戶進行交談並提供電子郵件ID期間，我們會解決該電子郵件ID是否存在已知潛在客戶記錄，並即時將該記錄用於個人化。 如果我們找到多個記錄，我們會即時合併它們。 此行為會針對對話方塊和對話流程實施。

### 從Marketo Engage同步沒有Cookie的銷售機會 {#syncing-leads-without-cookies}

先前，啟動Marketo Engage同步時，Dynamic Chat只會將已知的銷售機會與Marketo Engage的一或多個Cookie ID同步。 現在，所有已知的潛在客戶（無論是否有Cookie ID）都會同步至Dynamic Chat，並可用於個人化的交談。

### 將其他訪客資料傳遞至對話流程 {#pass-additional-visitor-data}

如果您透過其他管道（如表單或登入）擷取訪客資訊，現在可以直接將此資訊傳遞至Dynamic Chat。

![](assets/dynamic-chat-aug-2024-release-5.png)

### 重新整理推斷的資料 {#refreshed-inferred-data}

網站上的大多數交談都是與匿名訪客進行的。 您仍然可以透過推斷的資料來鎖定他們，而這有賴於訪客IP。 我們已更新IP資料庫和個別推斷資料，現在支援的IP是原來的四倍。

### 新增至代理程式瀏覽器通知的聲音 {#sound-added-to-agent-browser-notification}

將即時聊天指派給代理時，他們會收到瀏覽器通知。 但他們偶爾會看不見它們。 我們已新增[通知音效](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"}，以防止日後遺漏通知。

![](assets/dynamic-chat-aug-2024-release-6.png)

### 可在即時聊天期間更新潛在客戶設定檔 {#update-lead-profile-during-live-chat}

在即時聊天期間，代理程式想要擷取訪客的相關資訊並更新個別設定檔。 現在可以選擇更新潛在客戶與公司物件的屬性值。

![](assets/dynamic-chat-aug-2024-release-7.png)

## 2024 年 6 月發行版本 {#june-release}

**發行日期： 2024年6月6日**

### 對話式流量卡 {#conversational-flow-card}

運用對話流程卡，簡化對話方塊中流程的多個步驟。

範例：如果您的目標是透過多個對話方塊推動網路研討會註冊，則必須在具有該目標的所有對話方塊中重新建立相同的流程。 如果您必須更新任何詳細資訊，則必須一次編輯一個對話方塊。 由於有對話流量卡，情況已完全不同。

除了跨多個對話方塊重新利用流程之外，您還可以使用相同的轉變流程來觸發其他管道，例如表單和登陸頁面。

![](assets/dynamic-chat-june-2024-release-1.png)

### 使用量限制 {#usage-limits}

使用限制頁面會顯示重要資訊，例如封裝詳細資訊和使用限制狀態。

![](assets/dynamic-chat-june-2024-release-2.png)

## 2024 年 5 月發行 {#may-release}

**發行日期： 2024年5月15日**

### 預先核准的回應程式庫 {#pre-approved-response-library}

[建立行銷核准的資料庫](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} AI產生的問題和回答，以協助在幾分鐘內設定產生式AI聊天。

![](assets/dynamic-chat-may-2024-release-1.png)

### 未回答的問題 {#unanswered-questions}

[使用先前交談的未回答問題存放庫](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"}來產生新的預先核准回應，並維護包含最新資訊的回應資料庫。

![](assets/dynamic-chat-may-2024-release-2.png)

### 交談摘要 {#conversation-summaries}

[為銷售代理提供總結的交談](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"}，包括會議前的重要討論主題深入分析，以縮短準備時間，並更妥善地為銷售代理提供最新資訊。

![](assets/dynamic-chat-may-2024-release-3.png)

### GenAI銷售捷徑 {#genai-sales-shortcuts}

[以更快的方式提供即時聊天代理程式](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"}以存取AI產生的回應、編輯現有的已產生回應，並搜尋其他內容以在交談期間傳送給購買者。

![](assets/dynamic-chat-may-2024-release-4.png)

### 交談助理 {#conversation-assist}

透過行銷團隊預先核准的回應，協助銷售代理商在即時交談中正確回應。

### 交談輕推 {#conversation-nudges}

透過call-to-action輕推網頁訪客，推動對話結束。

<p>

## 2024 年 4 月發行版本 {#april-release}

**發行日期： 2024年4月23日**

### 交談流程現在可供所有使用者使用 {#conversational-flows-available-to-all-users}

允許合格的潛在客戶在提交表單後立即預約會議或與Sales聊天，讓您的表單和登入頁面更具對話性，並縮短銷售漏斗。Conversational Forms現在已完全可供所有Dynamic Chat使用者使用&#42;。

_&#42;先前提供試用功能，包含100個期限參與專案。 對話流程參與現在計入Select套件上使用者250個參與對話的每月限制。_

### 回呼函式 {#callback-functions}

[回撥函式](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"}可讓您在訪客參與Dynamic Chat對話時，收集Adobe Analytics或Google Analytics等外部系統中的Dynamic Chat分析事件。 您可以使用API註冊回呼來監聽事件，藉此啟用Dynamic Chat Analytics事件。 這可讓您在與其他關鍵資料（例如網站流量）相關時，以更整體的方式檢視Dynamic Chat參與。

### 即時代理程式可用性條件已新增到條件式分支 {#live-agent-availability-conditional-branching}

除了原生和自訂Marketo Engage欄位以外，您現在還可以使用條件式分支，根據代理程式可用性建立分支。 如果您只想讓訪客在有可用的即時代理程式時選擇與即時代理程式交談，這個功能會很有用。

![](assets/dynamic-chat-release-1.png)

### 智慧清單條件已新增到條件式分支 {#smart-list-condition}

在條件式分支中新增新的Marketo Engage智慧清單條件後，您可以根據已在Marketo Engage中建立的現有對象建立分支，而非在Dynamic Chat中定義對象分支條件。

![](assets/dynamic-chat-release-2.png)

### 對話流程的條件式分支 {#conditional-branching-for-conversational-flows}

我們今年早些時候發佈了對話的條件分支，現在您也可以利用對話流程中的條件分支！ 條件式分支可讓您根據不同條件在流程中建立分支。

### 對話流程的即時聊天 {#live-chat-for-conversational-flows}

我們在2023年發佈了對話的即時聊天功能，現在您也可以將即時聊天參與新增到對話流程中。 如果您搭配Marketo Engage表單使用對話流程，您現在可以允許合格訪客在表單提交後立即與即時代理程式聊天！

### 代理程式收件匣中最近的Marketo Engage活動 {#recent-marketo-engage-activities-in-agent-inbox}

我們已將最近的Marketo Engage活動新增到「代理程式收件匣」的「最近活動」區段，因此當網站訪客請求與代理程式聊天時，代理程式可以快速檢視該訪客最近是否參與了以下任何Marketo Engage活動（最近25個活動）：

* 已開啟的電子郵件
* 已造訪的網頁
* 已填寫表單
* 曾有過關鍵時刻

![](assets/dynamic-chat-release-3.png)

### 代理程式管理中的行事曆連線狀態 {#calendar-connection-status-in-agent-management}

管理員現在可以輕鬆檢視哪些具有會議預訂許可權的代理已連線他們在Dynamic Chat中的行事曆。 這可讓您確保整個銷售團隊都已連線，並準備好接受來自Dynamic Chat的會議要求。

![](assets/dynamic-chat-release-4.png)

### 代理程式行事曆設定中的最低通知設定 {#minimum-notice-setting-in-agent-calendar-configuration}

使用者回報網站訪客在預約會議時只需要10分鐘的預先通知，因此我們在代理程式行事曆設定中引進了最低通知設定，並將預設前置時間設定為24小時。

![](assets/dynamic-chat-release-5.png)

### 新增/移除使用者行為已更新 {#add-remove-user-behavior-updated}

有些使用者表示在Dynamic Chat中新增和移除代理程式時發生問題，因此我們進行了一些變更以解決這些問題。

當使用者新增到Admin Console並擁有即時聊天或會議預約許可權時，他們將立即出現在「代理管理」清單中，並可用於新增到對話方塊、對話流程、路由規則和團隊。

具有會議預約或即時聊天許可權的使用者從Admin Console中移除時，將會立即從Dynamic Chat中移除、無法再用於即時聊天或會議路由，且不再計入授許可權制。

### 改善交談層級報告效能 {#improved-conversation-level-report-performance}

「個別對話方塊」和「對話流量」層級報表現在可提供更有效且更準確的資料。 以前，載入對話方塊報表可能需要幾秒鐘的時間，而且資料偶爾會與全域效能報表不一致。 現在，您的個別對話方塊報表會立即載入，而且資料將一律與全域報表資料對齊。

![](assets/dynamic-chat-release-6.png)

### 許可權更新 {#permission-updates}

我們已清除Adobe Admin Console中的許可權結構和命名，讓許可權管理更直覺化。

* 「交談管理」類別現在稱為「交談」
* 「會議」類別現在稱為「活動」
* 「代理程式設定」類別現在稱為「代理程式」
* 「管理員設定」類別現在稱為「設定」
* 「即時交談」類別已移除，且所有即時聊天許可權已移至「代理程式」類別

![](assets/dynamic-chat-release-7.png)

### 支援代理程式收件匣中的超連結 {#support-for-hyperlinks-in-agent-inbox}

現在，當即時聊天代理程式與聊天中的訪客共用URL時，這些URL將會超連結，因此訪客只需按一下這些URL即可導覽至頁面，而不必將URL複製並貼到瀏覽器中。

### 在代理程式收件匣中輸入更新的金鑰行為 {#enter-key-behavior-updated-in-agent-inbox}

我們已切換「代理程式收件匣」中的傳回鍵行為，因此按Return或Enter鍵會傳送您的訊息，按Shift+Enter鍵會建立分行符號。

![](assets/dynamic-chat-release-8.png)

### 循環配置資源頁面已移除 {#round-robin-page-removed}

別擔心！ 循環配置資源路由仍然完全正常運作，而且運作方式與以往一樣。 我們剛才移除了在循環配置路由佇列中顯示經常不正確代理程式清單及其順序的頁面。

我們在2022年發行Dynamic Chat時，沒有提供即時聊天支援，只支援會議預訂，而且設計了循環配置選項路由頁面，充分考慮到會議預訂。 隨著去年即時聊天功能的推出，循環配置資源頁面已過時，因為它無法正確反映同時具有會議預約和即時聊天許可權之代理程式之間循環配置資源路由的更複雜性質。 我們探索了一些不同的選項來解決此問題，但最終決定完全移除它是最小化混淆的最佳選項。

![](assets/dynamic-chat-release-9.png)

## 2024 年 2 月發行版本 {#february-release}

**發行日期： 2024年2月22日**

### 對話頁面 {#conversations-page}

新的「交談」頁面提供了一站式服務，讓您檢視執行個體發生的所有交談（自動化和即時）記錄（來自已知和匿名潛在客戶），讓您更清楚瞭解客戶如何與您的對話、交談流程和即時代理進行互動。

![](assets/dynamic-chat-release-10.png)

### 全域控制面板中的日期範圍從90天增加到24個月 {#date-range-in-global-dashboard}

您詢問，我們已送達。 您現在可以在所有Analytics儀表板中檢視長達兩年的Dynamic Chat參與資料。

### 對話方塊中的條件分支 {#conditional-branching-in-dialogues}

條件式分支可讓您根據不同的條件，在對話方塊流程中建立分支。 現在，您可以根據Marketo Engage中的銷售機會和公司屬性，在相同對話方塊中向不同人員呈現不同的內容。

## 2024 年 1 月發行版本 {#january-release}

**發行日期： 2024年1月24日**

### 代理程式管理中的同時即時聊天限制設定 {#Concurrent-live-chat-limit-setting}

依預設，您執行個體中的每個即時聊天代理程式一次最多可以參與5個即時聊天工作階段。 我們在代理程式管理中引進了新的設定，可讓您將此限制從1調整為10。

![](assets/dynamic-chat-release-11.png)
