---
description: 動態聊天概述 — Marketo文檔 — 產品文檔
title: 動態聊天概述
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: c386d5ae542f4f19ba2acf6d2472a0c9d79c20a3
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# 動態聊天概述 {#dynamic-chat-overview}

動態聊天允許您利用易於使用的介面來針對訪問您網站的人和帳戶。 收集相關內容，如姓名、聯繫資訊和自由文本。 站點訪問者還可以預訂與銷售團隊的會議。 動態聊天活動和項目資料可用於向Marketo程式添加成員並觸發跨渠道活動。

>[!NOTE]
>
>動態聊天正在逐步推出，目前可用性有限。 此頁面將隨著通用性(GA)詳細資訊的出現而更新。

>[!TIP]
>
>訪問 [此頁](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) 查看動態聊天的教程視頻。

## 整合 {#integrations}

動態聊天的一個關鍵元件是它能夠與您的Marketo訂閱進行本機介面。 為了充分利用此整合的全部功能，您首先需要啟動資料同步。 根據Marketo資料庫的大小，初始資料可能需要24小時， [一次同步](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) 完成。

正在同步以下內容：

* 人員欄位資料
* 公司欄位資料
* 活動資料

## 對話框 {#dialogues}

對話框代表單個聊天項目。 將它想像成一個容器，其中包含您需要的所有內容，以便與網站訪問者進行有趣的聊天對話。 在每個對話框中，可以指定希望對話框顯示在哪個頁面上，希望該對話框顯示到誰，以及該對話框本身的內容和流。 此外，您還可以找到度量，以查看對話框的效能。 [瞭解有關對話框的詳細資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)。

## 配置 {#configuration}

在「配置」頁籤中，自定義各種對話框的外觀。 更改字型、顏色、響應時間等！ [瞭解有關配置的詳細資訊](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md)。

## 日曆 {#calendar}

在「日曆」頁籤中，連接您（Outlook或Gmail）的日曆，以便在聊天室中安排約會。 用戶的日曆連接到動態聊天后，該用戶將被添加到隊列，其日曆將可供網站訪問者安排約會。

您還可以自定義邀請的正文，當訪問者在用戶日曆上安排約會時，這些邀請將發送給訪問者。

## 會議 {#meetings}

在此，您將通過各種對話框看到網站訪問者安排的所有約會。 在此，您將找到預訂約會的人員的電子郵件地址、他們預訂約會的座席、安排約會的時間以及會議是否已經召開。

## 路由 {#routing}

您可以在此處查看連接日曆的所有代理的清單，以及向網站訪問者顯示這些代理的順序。 會議按循規蹈矩，所以如果你有五個探員和三號探員參加了最後一次會議，四號探員會得到下一個，然後是五號探員，然後是一號探員。

## 常見問題 {#faq}

**動態聊天是否允許即時聊天？**

不，它只利用預先確定的響應。

**我怎麼能瞄準匿名人？**

在對話框中，您需要使用 _人員電子郵件為空_ 屬性。

**是否支援AI/NLP功能？**

我們不支援AI/NLP功能。

**資料儲存多長時間用於報告？**

90天。

**「動態聊天」除了提供英語以外，還提供任何語言嗎？**

現在不行。

## 動態聊天中的限制 {#limits-in-dynamic-chat}

<table>
  <th>參數</th>
  <th>說明</th>
  <th>限制</th>
 <tr>
  <td>對話框總數</td>
  <td>對話總數（已發佈和草稿）</td>
  <td>500</td>
 </tr>
 <tr>
  <td>已發佈對話框</td>
  <td>保存的已發佈對話框數</td>
  <td>100</td>
 </tr>
 <tr>
  <td>每個對話框的目標URL</td>
  <td>可添加到單個對話框的目標URL數</td>
  <td>20</td>
 </tr>
 <tr>
  <td>每個對話框的屬性</td>
  <td>可添加到單個對話框的受眾標準的屬性數</td>
  <td>100</td>
 </tr>
 <tr>
  <td>組</td>
  <td>可添加到單個對話框的組數</td>
  <td>10</td>
 </tr>
 <tr>
  <td>每個組的屬性</td>
  <td>可添加到組的屬性數</td>
  <td>10</td>
 </tr>
 <tr>
  <td>卡</td>
  <td>每個對話框可添加到畫布的卡數</td>
  <td>500</td>
 </tr>
 <tr>
  <td>匿名潛在客戶資料保留期</td>
  <td>匿名潛在顧客資訊將保留多長時間而不進行任何接洽</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>目標活動保留期</td>
  <td>保留時間目標活動資料的量</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>文檔活動保留期</td>
  <td>保留文檔活動資料的時間量</td>
  <td>24個月</td>
 </tr>
 <tr>
  <td>對話框活動保留期</td>
  <td>保留與對話活動資料交互的時間量</td>
  <td>90天</td>
 </tr>
 <tr>
  <td>會議預訂活動保留期</td>
  <td>會議預訂活動的時間量將儲存在動態聊天中</td>
  <td>24個月</td>
 </tr>
</table>
