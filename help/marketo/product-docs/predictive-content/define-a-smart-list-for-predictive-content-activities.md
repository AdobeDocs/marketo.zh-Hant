---
unique-page-id: 10097873
description: 定義預測性內容活動的智慧型清單——行銷檔案——產品檔案
title: 定義預測性內容活動的智慧型清單
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# 定義預測性內容活動的智慧清單{#define-a-smart-list-for-predictive-content-activities}

>[!NOTE]
>
>視購買日期而定，您的Marketo訂閱可能包含Marketo Predictive Content或Content`<sup>AI</sup>`。 對於使用預測性內容的使用者，Marketo會在2018年4月30日之前啟用「內容`<sup>AI</sup>`分析」功能。 若要將這些功能保留在該日期之後，請連絡您的Marketo Customer Success Manager以升級至Marketo Content`<sup>AI</sup>`。

在智慧型促銷活動中定義智慧型清單時，您可以在觸發器和篩選器中使用預測性內容活動。 您可以透過[多媒體範本](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[內容建議列](enabling-predictive-content/enable-the-content-recommendation-bar.md)或電子郵件，針對任何點按預測性內容的人觸發動作。

1. 在智慧型促銷活動中，導覽至&#x200B;**智慧型清單**&#x200B;標籤。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >**深入探討**
   >
   >
   >智慧型清單可以做出令人驚艷的事。 進一步瞭解[智慧型清單深入探討](../../product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)。

1. 搜尋觸發器，然後將其拖放至畫布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有觸發器的智慧型促銷活動會在觸發器模式中執行。 它會根據觸發的事件和新增的篩選條件，一次在一個人上執行。

1. 按一下&#x200B;**名稱**&#x200B;下拉式清單並選取運算子。

   ![](assets/smart-list-dropdown-hands.png)

1. 定義觸發器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 添加&#x200B;**Type**&#x200B;約束。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 選擇智慧清單所需的源。

   ![](assets/pc-add-constraint.png)

1. 如果您使用電子郵件來源做為預測性內容，請在電子郵件**觸發器中新增**點按連結。 選擇您的電子郵件並添加&#x200B;**Is Predictive**&#x200B;約束，定義為&#x200B;**true**。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 視需要新增任何其他篩選器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在具有觸發器和篩選器的智慧型促銷活動中，觸發器會移至頂端。 觸發時，只有符合篩選條件的人才會瀏覽流程。

   >[!NOTE]
   >
   >如果有多個觸發器，當任一個觸發器被啟動時，人員會進入流程。

   [為批智慧促銷活動定義智慧清單](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [定義智慧型促銷活動的智慧型清單 |批次](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >    * [新增流量步驟至智慧型促銷活動](../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >    * [為Web個人化活動定義智慧清單](../../product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >    * [為網頁豐富式媒體啟用預測式內容](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >    * [啟用內容建議列](enabling-predictive-content/enable-the-content-recommendation-bar.md)


若要同時在一組人員上執行促銷活動，請學習如何。