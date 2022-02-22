---
description: 對話 — Marketo文檔 — 產品文檔
title: 對話框
exl-id: 5ec17ad0-6d56-4c06-a6ac-4c5771b2d91d
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# 對話框 {#dialogues}

對話是個別的聊天對話。 瞭解如何以視覺方式定制它們，確定它們所顯示的頁面，並決定說的內容以及看到的內容。

## 建立新對話框 {#create-a-new-dialogue}

1. 按一下 **對話框**。

   ![](assets/dialogues-1.png)

1. 按一下 **新建** 按鈕

   ![](assets/dialogues-2.png)

1. 輸入名稱（說明為可選），設定優先順序，然後按一下 **保存**。

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>優先順序確定當訪問者同時符合多個對話時將向其顯示哪個對話框。

## 受眾標準 {#audience-criteria}

與「Marketo智慧清單」類似，「受眾條件」屬性允許您定義目標受眾。 您可以使用推斷、人或公司屬性（或其組合）來瞄準已知或未知的人。

**已知人物**

有 _許多_ 要選擇的屬性組合。 在此示例中，我們針對所有 **有名人** 在一家員工超過50人的公司工作。

1. 抓住 **人員狀態** 將其拖到右側。

   ![](assets/dialogues-4.png)

1. _是_ 為預設設定。 在「選擇值」欄位中，鍵入CA（也可以按一下下拉清單並從清單中選擇）。

   ![](assets/dialogues-5.png)

1. 抓住 **公司規模** 屬性，並將其拖到 _拖放此處的屬性_。

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >也可以通過按一下屬性來選擇屬性 **+** 表徵圖

1. 按一下運算子下拉清單並選擇 **大於**。

   ![](assets/dialogues-7.png)

1. 鍵入50，然後按一下螢幕中的其他位置保存。

   ![](assets/dialogues-8.png)

就這樣！

**匿名人物**

有一種簡單的方法，可以專門針對尚未在資料庫中的人員。 在本例中，我們針對所有 **匿名者** 位於紐約地區。

1. 抓住 **人員電子郵件** 將其拖到右側。

   ![](assets/dialogues-9.png)

1. 按一下運算子下拉清單並選擇 **為空**。

   ![](assets/dialogues-10.png)

1. 抓住 **推斷狀態** 屬性，並將其拖到 _拖放此處的屬性_。

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >當有人訪問你的網站時， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 把它們餅乾，放進系統。 我們在一個特殊的資料庫中查找他們的IP，並推斷出各種好的資訊。

1. _是_ 為預設設定。 在「選擇值」(Select Values)欄位中，鍵入NY（也可以按一下下拉清單並從清單中選擇）。

   ![](assets/dialogues-12.png)

## 添加組 {#add-groups}

您也可以選擇對屬性進行分組，以防您希望具有所有特定屬性以及其它屬性的「全部或任何」。 可以添加多個組。

![](assets/dialogues-13.png)

![](assets/dialogues-14.png)

## 目標 {#target}

在此處輸入要顯示特定對話框的URL。

可接受的格式：

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>使用星號可充當「全收」的王牌。 所以 `https://*.website.com` 將該對話框放在站點的每一頁，包括子域(例如： `support.website.com`)。 和 `https://website.com/folder/*` 將對話框置於後續資料夾中的每個HTML頁(例如：在本例中，假設資料夾是「sports」，則：website.com/sports/baseball.html 、 website.com/sports/football.html等)。

## 流設計器 {#stream-designer}

流設計器包含您可以添加的不同卡，以形成聊天對話。

<table>
 <tr>
  <td><strong>訊息</strong></td>
  <td>在您想要生成無需響應的語句時使用(例如：「嗨！ 所有項目今天都減少了25%，代碼為SAVE25")。
</td>
 </tr>
 <tr>
  <td><strong>問題</strong></td>
  <td>當您想問多選題時使用，您將提供其可用回答(例如：你對哪種車感興趣？ 響應= SUV、緊湊型、卡車等)。</td>
 </tr>
 <tr>
  <td><strong>資訊捕獲</strong></td>
  <td>在要收集資訊時使用。 要選擇的三個欄位是「電子郵件地址」、「電話號碼」和「文本」（允許訪問者自行寫郵件）。</td>
 </tr>
 <tr>
  <td><strong>約會計畫程式</strong></td>
  <td>為訪問者提供可用日期日曆，以安排後續活動。 日曆可用性反映 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">下一個聯機代理</a>。</td>
 </tr>
 <tr>
  <td><strong>目標</strong></td>
  <td>這是訪客看不到的唯一一張牌。 您需要確定在特定聊天中的哪個點實現目標(例如：如果收集訪問者的電子郵件是您的目標，請將目標卡立即放在流中「資訊捕獲」之後)。</td>
 </tr>
</table>

**建立流**

有 _許多_ 可能的流組合。 我們來看一個例子 [本文](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)。

## 報告 {#reports}

在「報告」頁籤中，查看過去90天的資料。 每個類別定義如下。

<table>
 <tr>
  <td><strong>觸發總數</strong></td>
  <td>每次訪問者符合/顯示對話框時遞增。
</td>
 </tr>
 <tr>
  <td><strong>已訂</strong></td>
  <td>每次訪問者按一下聊天機定位點以開啟對話框時遞增。</td>
 </tr>
 <tr>
  <td><strong>已完成</strong></td>
  <td>每次訪問者到達對話框中任何分支的末尾時遞增。</td>
 </tr>
 <tr>
  <td><strong>已捕獲人員</strong></td>
  <td>每次訪問者在對話框流中提供有效電子郵件地址時遞增。</td>
 </tr>
 <tr>
  <td><strong>已預訂的會議</strong></td>
  <td>每次訪問者通過聊天機成功安排約會時遞增。</td>
 </tr>
 <tr>
  <td><strong>已達目標</strong></td>
  <td>每次訪問者在任何對話框流中到達目標時遞增。</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>[建立流](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)
