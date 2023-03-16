---
description: Dynamic Chat概述 — Marketo檔案 — 產品檔案
title: 動態聊天概述
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 5cd5873132e38d7adea02739da39aebeb3979124
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 2%

---

# 動態聊天概述 {#dynamic-chat-overview}

動態聊天功能可讓您利用簡單易用的介面，將目標同時鎖定在造訪您網站的人員和帳戶。 收集相關內容，例如姓名、聯繫資訊和自由文本。 網站訪客也可以預訂與您的銷售團隊的會議。 動態聊天活動和參與資料可用來新增成員至Marketo方案並觸發跨通道活動。

>[!NOTE]
>
>Dynamic Chat正在逐步推出，目前可用性有限。 本頁將隨正式發行(GA)詳細資訊的提供而更新。

>[!TIP]
>
>瀏覽 [本頁](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) 觀看動態聊天的教學課程影片。

## 整合 {#integrations}

Dynamic Chat的一個關鍵元件是其與Marketo訂閱原生介面的功能。 若要充分運用這項整合的完整功能，您必須先啟動資料同步。 視您的Marketo資料庫大小而定，初始資料可能需要24小時， [一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) 完成。

已同步下列項目：

* 人員欄位資料
* 公司欄位資料
* 活動資料

## 對話 {#dialogues}

對話方塊代表單一聊天參與。 您可以將其想像成容器，內含您與網站訪客進行有趣的聊天對話所需的所有內容。 在每個對話框中，可以指定希望對話框顯示在哪個頁面上、希望向誰顯示對話框，以及對話框本身的內容和流。 此外，您還可以找到量度，以了解對話方塊的執行成效。 [深入了解對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## 設定 {#configuration}

在「配置」頁簽中，自定義各種對話框的外觀和風格。 變更字型、顏色、回應時間等！ [進一步了解配置](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## 日曆 {#calendar}

連接您的Outlook或Gmail日曆，以用於動產中的約會排程。 [進一步了解日曆](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## 會議 {#meetings}

這是網站訪客透過各種對話方塊排程的所有約會。 [進一步了解會議](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## 路由 {#routing}

您可以在此處查看已連接其日曆的所有座席的清單，向網站訪客顯示這些座席的順序，以及建立自定義路由規則。 [進一步了解路由](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## 常見問題集 {#faq}

**我可以在公司網站上的任何地方安裝動態聊天嗎？還是只能在Marketo登陸頁面上運作？**

Dynamic Chat JavaScript程式碼片段可安裝在任何網站和Marketo登陸頁面上。

**資料儲存多久以用於報告？**

90天(請參閱完整限制清單 [low](#limits-in-dynamic-chat))。

**動態聊天是否允許即時聊天？**

不會，它只會使用預先決定的回應。

**Dynamic Chat是否支援英語以外的任何語言？**

是. 動態聊天支援下列語言：法文、德文、日文、西班牙文、義大利文、巴西葡萄牙文、韓文、簡體中文和繁體中文。 了解更多 [下文](#changing-the-language).

**您是否支援AI/NLP功能？**

我們不支援AI/NLP功能。

**如何鎖定匿名人員？**

在對話方塊中，您需要使用 _人員電子郵件為空_ 屬性。

## 變更語言 {#changing-the-language}

請依照下列步驟變更您的動態聊天語言。

>[!IMPORTANT]
>
>在設定檔層級變更您的語言將會變更 _all_ Experience Cloud應用程式，而不只是動態聊天。

1. 在您的Experience Cloud帳戶中，按一下設定圖示並選擇 **偏好設定**.

   ![](assets/dynamic-chat-overview-1.png)

1. 按一下您電子郵件地址下方的目前語言。

   ![](assets/dynamic-chat-overview-2.png)

1. 選擇您的新語言（第二種語言為選用語言），然後按一下 **儲存**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >有幾十種語言可供選擇，但Dynamic Chat僅支援下列語言：英文、法文、德文、日文、西班牙文、義大利文、巴西葡萄牙文、韓文、簡體中文和繁體中文。

當您更新語言時，應用程式本身中的所有項目都會變更，除了您個人填入的字詞（例如串流回應）。

## 動態聊天的限制 {#limits-in-dynamic-chat}

<table>
  <th>參數</th>
  <th>說明</th>
  <th>限制</th>
 <tr>
  <td>對話框總數</td>
  <td>對話次數（已發佈和草稿）</td>
  <td>500</td>
 </tr>
 <tr>
  <td>日曆總計</td>
  <td>連接的日曆數</td>
  <td>25</td>
 </tr>
 <tr>
  <td>使用者總數（管理員和行銷使用者）</td>
  <td>每個動態聊天實例允許的合併用戶數</td>
  <td>50</td>
 </tr>
 <tr>
  <td>已發佈的對話方塊</td>
  <td>已保存的已發佈對話框數</td>
  <td>100</td>
 </tr>
 <tr>
  <td>每個對話方塊的Target URL</td>
  <td>可新增至單一對話方塊的Target URL數量</td>
  <td>20</td>
 </tr>
 <tr>
  <td>每個對話框的屬性</td>
  <td>可新增至單一對話方塊對象條件的屬性數量</td>
  <td>100</td>
 </tr>
 <tr>
  <td>群組</td>
  <td>可添加到單個對話框的組數</td>
  <td>10</td>
 </tr>
 <tr>
  <td>每個組的屬性</td>
  <td>可添加到組的屬性數</td>
  <td>10</td>
 </tr>
 <tr>
  <td>卡片</td>
  <td>每個對話方塊可新增至畫布的卡片數</td>
  <td>500</td>
 </tr>
 <tr>
  <td>匿名銷售機會資料保留期</td>
  <td>將保留無任何參與的匿名銷售機會資訊的持續時間</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>目標活動保留期</td>
  <td>保留目標活動資料的時間量</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>文檔活動保留期</td>
  <td>保留文檔活動資料的時間量</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>與對話活動保留期互動</td>
  <td>保留與Dialog活動資料互動的時間量</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>會議預訂活動保留期</td>
  <td>會議預訂活動將儲存在動態聊天中的時間量</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>參與的對話</td>
  <td>每月網站訪客可參與的聊天對話數</td>
  <td>250</td>
 </tr>
 <tr>
  <td>觸發的對話</td>
  <td>每月可向Web訪客顯示的聊天對話數</td>
  <td>25,000</td>
 </tr>
</table>
