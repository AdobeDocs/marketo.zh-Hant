---
description: Dynamic Chat概述 — Marketo檔案 — 產品檔案
title: Dynamic Chat概觀
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 4%

---

# [!DNL Dynamic Chat] 概觀 {#dynamic-chat-overview}

Dynamic Chat可讓您運用易用的介面，將目標同時鎖定於造訪您網站的訪客和帳戶。 收集相關內容，例如姓名、聯絡資訊和任意文字。 網站訪客也可以與即時代理聊天，甚至預約與您的銷售團隊的會議。 Dynamic Chat活動和參與資料可用來將成員新增至Marketo方案並觸發跨頻道活動。

>[!TIP]
>
>請造訪[此頁面](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html?lang=zh-Hant){target="_blank"}，檢視Dynamic Chat的教學課程影片。

## 整合 {#integrations}

Dynamic Chat的主要元件是原生介面與您的Marketo訂閱的功能。 為了善用此整合的完整功能，您首先需要啟動資料同步。 視您的Marketo資料庫大小而定，完成初始[一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"}最多可能需要24小時的資料。

以下專案已同步：

* 個人欄位資料
* 公司欄位資料
* 活動資料

## 對話 {#dialogues}

對話方塊代表單一聊天專案。 將其視為一個容器，其中包含您為網站訪客提供引人入勝的聊天對話方塊所需的所有內容。 在每個對話方塊中，您可以指定您希望對話方塊顯示的頁面、顯示的對象，以及對話方塊本身的內容和流程。 此外，您可以尋找量度，以檢視對話方塊的執行狀況。 [進一步瞭解對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}。

## 設定 {#configuration}

在「組態」標籤中，自訂各種對話方塊的外觀和風格。 變更字型、顏色、回應時間等！ [進一步瞭解設定](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}。

## 行事曆 {#calendar}

連線您的Outlook或Gmail行事曆，以用於聊天機器人中的約會排程。 [進一步瞭解行事曆](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## 會議 {#meetings}

您將在這裡看到網站訪客透過各種對話方塊排程的所有約會。 [進一步瞭解會議](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## 路由 {#routing}

您可以在此處檢視已連線其行事曆的所有代理程式清單、其向網站訪客呈現的順序，以及建立自訂路由規則。 [進一步瞭解路由](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## 即時聊天 {#live-chat}

提供合格的網頁訪客，透過[即時交談](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}與銷售代表連絡。

## 交談流程 {#conversational-flow}

[設計訪客可以根據您指定的動作（例如，填寫表單、按一下連結等）觸發的交談](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}。

## 生成式 AI {#generative-ai}

Adobe Dynamic Chat中的[產生式AI](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"}會即時處理意圖訊號、使用者偏好設定和過去行為，以便為聊天訪客產生相關的個人化訊息。

## 變更語言 {#changing-the-language}

請依照下列步驟變更您的Dynamic Chat語言。

>[!IMPORTANT]
>
>在設定檔層級變更您的語言將會變更&#x200B;_所有_&#x200B;個Experience Cloud應用程式的語言，而不僅僅是[!DNL Dynamic Chat]。

1. 在您的Experience Cloud帳戶中，按一下設定圖示並選擇&#x200B;**[!UICONTROL Preferences]**。

   ![](assets/dynamic-chat-overview-1.png)

1. 按一下您電子郵件地址下的目前語言。

   ![](assets/dynamic-chat-overview-2.png)

1. 選擇您的新語言（第二種語言是選擇性的），然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >有幾十種語言可供選擇，不過[!DNL Dynamic Chat]僅支援下列語言：英文、法文、德文、日文、西班牙文、義大利文、巴西葡萄牙文、韓文、簡體中文和繁體中文。

當您更新語言時，除了您親自填入的字詞之外（例如資料流回應），應用程式本身中的所有內容都會變更。

## Dynamic Chat資料保留限制 {#dynamic-chat-data-retention-limits}

以下只是Dynamic Chat中的部分限制/引數。 如需完整清單，請參閱Marketo Engage [產品說明頁面](https://helpx.adobe.com/tw/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}。

<table>
  <th>資料類型</th>
  <th>保留期間</th>
 <tr>
  <td>無任何參與的匿名銷售機會</td>
  <td>90 天</td>
 </tr>
 <tr>
  <td>目標活動</td>
  <td>24 個月</td>
 </tr>
 <tr>
  <td>檔案活動</td>
  <td>24 個月</td>
 </tr>
 <tr>
  <td>與對話方塊活動互動</td>
  <td>90 天</td>
 </tr>
 <tr>
  <td>會議預約活動</td>
  <td>24 個月</td>
 </tr>
</table>

## 常見問題集 {#faq}

請參閱[Dynamic Chat常見問題集](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}。
