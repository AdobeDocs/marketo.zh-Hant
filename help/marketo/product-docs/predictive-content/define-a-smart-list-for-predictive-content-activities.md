---
unique-page-id: 10097873
description: 定義預測性內容活動的智慧清單 — Marketo檔案 — 產品檔案
title: 定義預測內容活動的智慧清單
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 定義預測內容活動的智慧清單 {#define-a-smart-list-for-predictive-content-activities}

在智慧型行銷活動中定義智慧清單時，您可以在觸發器和篩選器中使用預測性內容活動。 您可以針對透過 [多媒體範本](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), [內容建議列](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)，或 [電子郵件](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. 在您的智慧型行銷活動中，導覽至 **智慧清單** 標籤。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >聰明的清單可以做出令人驚嘆的事情。 了解更多 [智慧型清單深入探索](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. 搜尋觸發器，然後將其拖放至畫布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有觸發器的智慧型行銷活動會在觸發模式中執行。 它會根據觸發的事件和新增的篩選器，一次在一個人上執行。

1. 按一下 **名稱** 下拉式清單中選取運算子。

   ![](assets/smart-list-dropdown-hands.png)

1. 定義觸發器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 新增 **類型** 限制。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 選擇智慧清單所需的源。

   ![](assets/pc-add-constraint.png)

1. 如果您使用電子郵件來源來預測內容，請新增 **點按電子郵件中的連結** 觸發。 選取您的電子郵件並新增 **可預測** 約束，定義為 **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 視需要新增任何其他篩選器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在同時具有觸發器和篩選器的智慧型行銷活動中，觸發器會排在頂端。 觸發時，只有符合篩選條件的人才會瀏覽流量。

   >[!NOTE]
   >
   >如果有多個觸發器，如果有任何一個觸發器啟動，人員會進入流程。

   若要同時在一組人員上執行行銷活動，請了解如何 [為批次智慧型促銷活動定義智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [定義智慧促銷活動的智慧清單 |批](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [新增流量步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [為Web個人化活動定義智慧清單](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [為Web多媒體啟用預測性內容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [啟用內容建議列](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

