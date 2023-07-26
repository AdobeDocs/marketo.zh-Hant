---
description: Dynamic Chat概述 — Marketo檔案 — 產品檔案
title: Dynamic Chat概觀
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 2%

---

# Dynamic Chat概觀 {#dynamic-chat-overview}

Dynamic Chat可讓您運用易用的介面，將目標同時鎖定於造訪您網站的訪客和帳戶。 收集相關內容，例如姓名、聯絡資訊和任意文字。 網站訪客也可以預約與您的銷售團隊開會。 Dynamic Chat活動和參與資料可用來將成員新增至Marketo方案，並觸發跨頻道活動。

>[!NOTE]
>
>Dynamic Chat正在逐步推出，目前可用性有限。 此頁面將會在可供使用時以一般可用性(GA)詳細資訊更新。

>[!TIP]
>
>造訪 [此頁面](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) 以檢視Dynamic Chat的教學課程影片。

## 整合 {#integrations}

Dynamic Chat的一個重要元件，是能夠與您的Marketo訂閱原生介面。 為了善用此整合的完整功能，您首先需要啟動資料同步。 根據Marketo資料庫的大小，初始的資料可能最多需要24小時的時間。 [一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) 完成。

以下專案已同步：

* 個人欄位資料
* 公司欄位資料
* 活動資料

## 對話 {#dialogues}

對話方塊代表單一聊天專案。 將其視為一個容器，其中包含您為網站訪客提供引人入勝的聊天對話方塊所需的所有內容。 在每個對話方塊中，您可以指定您希望對話方塊顯示的頁面、顯示的對象，以及對話方塊本身的內容和流程。 此外，您可以尋找量度，以檢視對話方塊的執行狀況。 [深入瞭解對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## 設定 {#configuration}

在「組態」標籤中，自訂各種對話方塊的外觀和風格。 變更字型、顏色、回應時間等！ [進一步瞭解設定](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## 行事曆 {#calendar}

連線您的Outlook或Gmail行事曆，以用於聊天機器人中的約會排程。 [深入瞭解行事曆](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## 會議 {#meetings}

您將在這裡看到網站訪客透過各種對話方塊排程的所有約會。 [進一步瞭解會議](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## 路由 {#routing}

您可以在此處檢視已連線其行事曆的所有代理程式清單、其向網站訪客呈現的順序，以及建立自訂路由規則。 [進一步瞭解路由](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## 常見問題集 {#faq}

**我可以在公司網站上的任何地方安裝Dynamic Chat，還是只能在Marketo登陸頁面上使用？**

Dynamic ChatJavaScript程式碼片段可安裝在任何網站以及Marketo登陸頁面上。

**資料會儲存多久以用於報告？**

90天（請參閱完整的限制清單） [以下](#limits-in-dynamic-chat))。

**Dynamic Chat允許即時聊天嗎？**

不會，只會使用預先決定的回應。

**Dynamic Chat是否支援英語以外的任何語言？**

是. Dynamic Chat支援下列語言：法文、德文、日文、西班牙文、義大利文、巴西葡萄牙文、韓文、簡體中文和繁體中文。 進一步瞭解 [區段如下](#changing-the-language).

**您支援AI/NLP功能嗎？**

我們不支援AI/NLP功能。

**如何鎖定匿名人員？**

在對話方塊中，您需要使用 _個人電子郵件是空的_ 屬性。

## 變更語言 {#changing-the-language}

請依照下列步驟變更您的Dynamic Chat語言。

>[!IMPORTANT]
>
>在設定檔層級變更您的語言將會變更 _全部_ Experience Cloud應用程式，而不僅僅是Dynamic Chat。

1. 在您的Experience Cloud帳戶中，按一下設定圖示並選擇 **偏好設定**.

   ![](assets/dynamic-chat-overview-1.png)

1. 按一下您電子郵件地址下的目前語言。

   ![](assets/dynamic-chat-overview-2.png)

1. 選擇您的新語言（第二種語言為選用），然後按一下 **儲存**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >有幾十種語言可供選擇，但Dynamic Chat僅支援下列語言：英文、法文、德文、日文、西班牙文、義大利文、巴西葡萄牙文、韓文、簡體中文和繁體中文。

當您更新語言時，除了您親自填入的字詞之外（例如資料流回應），應用程式本身中的所有內容都會變更。

## Dynamic Chat限制 {#limits-in-dynamic-chat}

<table>
  <th>引數</th>
  <th>說明</th>
  <th>限制</th>
 <tr>
  <td>對話方塊總數</td>
  <td>對話方塊數目（已發佈及草稿）</td>
  <td>500</td>
 </tr>
 <tr>
  <td>行事曆總數</td>
  <td>連線的行事曆數目</td>
  <td>25</td>
 </tr>
 <tr>
  <td>使用者總數（管理員和行銷使用者）</td>
  <td>每個Dynamic Chat例項允許的合併使用者數</td>
  <td>50</td>
 </tr>
 <tr>
  <td>已發佈對話方塊</td>
  <td>已儲存的已發佈對話方塊數目</td>
  <td>100</td>
 </tr>
 <tr>
  <td>每個對話方塊的目標URL</td>
  <td>可新增至單一對話方塊的目標URL數量</td>
  <td>20</td>
 </tr>
 <tr>
  <td>每個對話方塊的屬性</td>
  <td>單一對話方塊可新增至對象條件的屬性數量</td>
  <td>100</td>
 </tr>
 <tr>
  <td>群組</td>
  <td>可新增至單一對話方塊的群組數量</td>
  <td>10</td>
 </tr>
 <tr>
  <td>每個群組的屬性</td>
  <td>可新增至群組的屬性數量</td>
  <td>10</td>
 </tr>
 <tr>
  <td>卡片</td>
  <td>每個對話方塊可新增到畫布的卡片數量</td>
  <td>500</td>
 </tr>
 <tr>
  <td>匿名潛在客戶資料保留期</td>
  <td>沒有任何參與的匿名潛在客戶資訊將保留多久的時間</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>目標活動保留期</td>
  <td>保留目標活動資料的時間量</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>檔案活動保留期</td>
  <td>檔案活動資料的保留時間</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>與對話方塊活動保留期間互動</td>
  <td>保留與對話方塊活動資料互動的時間長度</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>會議預約活動保留期間</td>
  <td>會議預約活動將以Dynamic Chat儲存的時間長度</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>已參與的交談</td>
  <td>每個月可由Web訪客參與的聊天對話數</td>
  <td>250</td>
 </tr>
 <tr>
  <td>對話已觸發</td>
  <td>每個月可顯示給Web訪客的聊天對話次數</td>
  <td>25,000</td>
 </tr>
</table>
