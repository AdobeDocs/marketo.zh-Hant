---
unique-page-id: 7513680
description: 自動提醒可能重複的人員 — Marketo檔案 — 產品檔案
title: 自動提供可能重複人員的警報
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 50fc46312d2c7c25556994fad4e118c01cf92fc0
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 自動提供可能重複人員的警報 {#automate-an-alert-for-possible-duplicate-people}

是否要在每次建立可能的重複人員時發出警報？ 以下說明如何設定智慧型行銷活動。

1. [建立新的智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}。 定義下列智慧清單：

* 觸發： **已建立人員**
* 篩選： **重複欄位。** 欄位名稱 **為全名**

   ![](assets/automate-an-alert-1.png)

   >[!TIP]
   >
   >有創意。 實驗不同的場，得到更好的濾波效果。

1. 在流程步驟中，選擇 [傳送警報](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target=&quot;_blank&quot;}流操作。

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >使用 [傳送警報資訊Token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}，以在CRM中包含連結至人員。

   >[!CAUTION]
   >
   >如果您匯入大型清單，可能會同時收到一堆警報！
   >
   >另外，兩個同名的人並不自動表示他們是同一個人。

1. 在 **排程** 標籤。

   ![](assets/automate-an-alert-3.png)

就這樣！ 每次在Marketo中建立現有全名的新人員時，都會觸發此智慧型促銷活動。

>[!MORELIKETHIS]
>
>[查找和合併重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
