---
unique-page-id: 10097873
description: 定義預測性內容活動的智慧清單 — Marketo檔案 — 產品檔案
title: 定義預測性內容活動的智慧清單
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 定義預測性內容活動的智慧清單 {#define-a-smart-list-for-predictive-content-activities}

當您在智慧行銷活動中定義智慧清單時，可以在觸發器和篩選器中使用預測性內容活動。 任何透過[Rich Media範本](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[內容建議列](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)或[電子郵件](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md)按一下預測性內容的人，都可以觸發動作。

1. 在您的智慧行銷活動中，導覽至「**[!UICONTROL Smart List]**」標籤。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >智慧清單可以做一些令人驚異的事情。 進一步瞭解[智慧清單深入探討](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)。

1. 搜尋觸發程式，然後將其拖放到畫布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有觸發器的智慧行銷活動會在觸發模式下執行。 它會根據觸發的事件和新增的篩選器，一次只對一個人執行。

1. 按一下&#x200B;**[!UICONTROL Name]**&#x200B;下拉式清單，然後選取運運算元。

   ![](assets/smart-list-dropdown-hands.png)

1. 定義觸發器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 新增&#x200B;**[!UICONTROL Type]**&#x200B;條件約束。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 選取您需要的智慧清單來源。

   ![](assets/pc-add-constraint.png)

1. 如果您將電子郵件來源用於預測性內容，請新增&#x200B;**[!UICONTROL Clicks Link in Email]**&#x200B;觸發器。 選取您的電子郵件並新增定義為&#x200B;**[!UICONTROL Is Predictive]**&#x200B;的&#x200B;**[!UICONTROL true]**&#x200B;條件約束。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 視需要新增任何其他篩選器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在同時具有觸發器和篩選器的智慧行銷活動中，觸發器位於頂端。 觸發時，只有符合篩選條件的人才會通過流程。

   >[!NOTE]
   >
   >使用多個觸發器時，如果任何一個觸發器啟動，則人員會進入流程。

   若要對一組人員同時執行行銷活動，瞭解如何[為批次智慧行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)定義智慧清單。

   >[!MORELIKETHIS]
   >
   >* [定義智慧行銷活動的智慧清單 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [將流程步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [定義網路Personalization活動的智慧清單](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [啟用Web Rich Media的預測內容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [啟用內容建議列](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
