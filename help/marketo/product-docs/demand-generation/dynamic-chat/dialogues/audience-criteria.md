---
description: 受眾標準 — Marketo文檔 — 產品文檔
title: 受眾標準
source-git-commit: 38e65efc50f7f5e7a2a3dbe91035327007475721
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 受眾標準 {#audience-criteria}

與「Marketo智慧清單」類似，「受眾條件」屬性允許您定義目標受眾。 您可以使用推斷、人或公司屬性（或其組合）來瞄準已知或未知的人。

**已知人物**

有 _許多_ 要選擇的屬性組合。 在此示例中，我們針對所有 **有名人** 在一家員工超過50人的公司工作。

1. 抓住 **人員狀態** 將其拖到右側。

   ![](assets/audience-criteria-1.png)

1. _是_ 為預設設定。 在「選擇值」欄位中，鍵入CA（也可以按一下下拉清單並從清單中選擇）。

   ![](assets/audience-criteria-2.png)

1. 抓住 **公司規模** 屬性，並將其拖到 _拖放此處的屬性_。

   ![](assets/audience-criteria-3.png)

   >[!NOTE]
   >
   >也可以通過按一下屬性來選擇屬性 **+** 表徵圖

1. 按一下運算子下拉清單並選擇 **大於**。

   ![](assets/audience-criteria-4.png)

1. 鍵入50，然後按一下螢幕中的其他位置保存。

   ![](assets/audience-criteria-5.png)

就這樣！

**匿名人物**

有一種簡單的方法，可以專門針對尚未在資料庫中的人員。 在本例中，我們針對所有 **匿名者** 位於紐約地區。

1. 抓住 **人員電子郵件** 將其拖到右側。

   ![](assets/audience-criteria-6.png)

1. 按一下運算子下拉清單並選擇 **為空**。

   ![](assets/audience-criteria-7.png)

1. 抓住 **推斷狀態** 屬性，並將其拖到 _拖放此處的屬性_。

   ![](assets/audience-criteria-8.png)

   >[!NOTE]
   >
   >當有人訪問你的網站時， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 把它們餅乾，放進系統。 我們在一個特殊的資料庫中查找他們的IP，並推斷出各種好的資訊。

1. _是_ 為預設設定。 在「選擇值」(Select Values)欄位中，鍵入NY（也可以按一下下拉清單並從清單中選擇）。

   ![](assets/audience-criteria-9.png)

## 添加組 {#add-groups}

您也可以選擇對屬性進行分組，以防您希望具有所有特定屬性以及其它屬性的「全部或任何」。 可以添加多個組。

![](assets/audience-criteria-10.png)

![](assets/audience-criteria-11.png)

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

>[!MORELIKETHIS]
>
>* [建立對話框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;
>* [流設計器](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;
>* [報告](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;

