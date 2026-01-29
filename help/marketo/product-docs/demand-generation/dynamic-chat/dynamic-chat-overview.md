---
description: Dynamic Chat 概觀 - Marketo 文件 - 產品文件
title: Dynamic Chat 概觀
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '587'
ht-degree: 100%

---

# [!DNL Dynamic Chat] 概觀 {#dynamic-chat-overview}

Dynamic Chat 讓您可運用易用的介面，將造訪您網站的訪客和帳戶同時鎖定為目標。收集相關內容，例如姓名、聯絡資訊和任意文字。網站訪客也可以與線上專員聊天，甚至與您的銷售團隊預約會議。Dynamic Chat 活動和參與資料可用於將成員新增至 Marketo 方案並觸發跨管道活動。

>[!TIP]
>
>請造訪[此頁面](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html?lang=zh-Hant){target="_blank"}，以檢視 Dynamic Chat 的教學課程影片。

## 整合 {#integrations}

Dynamic Chat 的關鍵元件為其與您的 Marketo 訂閱建立原生介面的能力。為了善用此整合的完整功能，您首先需要啟動資料同步。依您的 Marketo 資料庫大小而定，資料完成初始、[一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"}的時間可能需要最多 24 小時。

以下項目已同步：

* 個人欄位資料
* 公司欄位資料
* 活動資料

## 對話 {#dialogues}

對話代表單一聊天互動。不妨將其視為一個容器，其中包含為網站訪客提供引人入勝的聊天對話所需的所有內容。在每個對話中，您可以指定您希望對話顯示的頁面、顯示的對象，以及對話本身的內容與流程。此外，您可以尋找量度，以查看對話的執行狀況。[了解更多有關「對話」的資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}。

## 設定 {#configuration}

在「設定」索引標籤中，自訂各種對話的外觀。變更字型、顏色、回應時間等！[了解更多有關「設定」的資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}.

## 行事曆 {#calendar}

和您的 Outlook 或 Gmail 行事曆連線，以用於聊天機器人中的約會排程。[了解更多有關「行事曆」的資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## 會議 {#meetings}

您會在這裡看到網站訪客透過各種對話所排程的所有約會。[了解更多有關「會議」的資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## 路由 {#routing}

您可以在這裡查看已與其行事曆連線的所有代理程式清單、其向網站訪客呈現的順序，並建立自訂路由規則。[了解更多有關「路由」的資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}。

## 即時聊天 {#live-chat}

提供符合資格的網頁訪客，以透過[即時聊天](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}與銷售代表聯絡。

## 交談流程 {#conversational-flow}

[設計交談](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}，可由訪客依據您指定的動作 (例如，填寫表單、點按連結等) 來觸發。

## 生成式 AI {#generative-ai}

Adobe Dynamic Chat 中的[生成式 AI](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"}可即時處理意圖訊號、使用者偏好設定和過去行為，以便為聊天訪客產生相關的個人化訊息。

## 變更語言 {#changing-the-language}

請依照下列步驟變更您的 Dynamic Chat 語言。

>[!IMPORTANT]
>
>在設定檔層級變更您的語言後，_所有_ Experience Cloud 應用程式的語言都會變更，而不僅限於 [!DNL Dynamic Chat]。

1. 在您的 Experience Cloud 帳戶中，按一下設定圖示並選擇 **[!UICONTROL Preferences]**。

   ![](assets/dynamic-chat-overview-1.png)

1. 按一下您電子郵件地址下的目前語言。

   ![](assets/dynamic-chat-overview-2.png)

1. 選擇您的新語言 (第二種語言為選用)，然後按一下 **[!UICONTROL Save]**。

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >有幾十種語言可供選擇，不過 [!DNL Dynamic Chat] 僅支援下列語言：英文、法文、德文、日文、西班牙文、義大利文、巴西葡萄牙文、韓文、簡體中文和繁體中文。

當您更新語言時，除了您已親自填入的字詞 (例如資料流回覆) 外，應用程式本身中的所有內容都會變更。

## Dynamic Chat 資料保留限制 {#dynamic-chat-data-retention-limits}

以下只是 Dynamic Chat 中的部分限制/參數。如需完整清單，請參閱 Marketo Engage [產品說明頁面](https://helpx.adobe.com/tw/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}。

<table>
  <th>資料類型</th>
  <th>保留期間</th>
 <tr>
  <td>無任何參與的匿名銷售線索</td>
  <td>90 天</td>
 </tr>
 <tr>
  <td>目標活動</td>
  <td>24 個月</td>
 </tr>
 <tr>
  <td>文件活動</td>
  <td>24 個月</td>
 </tr>
 <tr>
  <td>與對話活動互動</td>
  <td>90 天</td>
 </tr>
 <tr>
  <td>會議預約活動</td>
  <td>24 個月</td>
 </tr>
</table>

## 常見問題集 {#faq}

請參閱 [Dynamic Chat 常見問題集](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}。
