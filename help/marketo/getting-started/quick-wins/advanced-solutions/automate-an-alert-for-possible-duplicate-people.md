---
unique-page-id: 7513680
description: 自動發出可能重複的人員警報 — Marketo文檔 — 產品文檔
title: 自動發出可能重複的人員警報
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 自動發出可能重複的人員警報 {#automate-an-alert-for-possible-duplicate-people}

是否希望每次建立可能的重複人員時都發出警報？ 下面是如何建立一個智慧營銷活動來實現它。

1. [建立新的智慧市場活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}。 定義以下智慧清單：

* 觸發器： **建立人員**
* 篩選器： **重複欄位。** 欄位名稱 **是全名**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >有創意。 對不同場進行實驗，得到較好的濾波效果。

1. 在流步驟中，選擇 [發送警報](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target=&quot;_blank&quot;}流操作。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >使用 [發送警報資訊令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}，以在CRM中包含指向該人員的連結。

   >[!CAUTION]
   >
   >如果導入大清單，您可能同時收到大量警報！
   >
   >另外，兩個同名的人並不自動意味著他們是同一個人。

1. 在 **計畫** 頁籤。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

就這樣！ 每次在Marketo建立新的全名人員時，都會觸發此智慧活動。

>[!MORELIKETHIS]
>
>[查找並合併重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;
