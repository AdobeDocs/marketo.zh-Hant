---
unique-page-id: 1146942
description: 定義Smart Campaign的智慧清單 | 觸發器 — Marketo檔案 — 產品檔案
title: 定義Smart Campaign的智慧清單 | 觸發
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 定義Smart Campaign的智慧清單 | 觸發 {#define-smart-list-for-smart-campaign-trigger}

透過新增觸發程式，根據即時事件逐人執行Smart Campaign。

>[!CAUTION]
>
>對作用中行銷活動進行智慧清單或流量步驟編輯可能會破壞其功能。 如果您選擇這麼做，請謹慎操作。

1. 在您的Smart Campaign中，按一下&#x200B;**[!UICONTROL 智慧清單]**&#x200B;索引標籤。

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. 搜尋所需的觸發器，並將其拖放到畫布上。

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >具有觸發程式的Smart Campaign會在&#x200B;_觸發程式_&#x200B;模式中執行。 它會根據觸發的事件和任何其他篩選器，一次只對一個人執行。

   >[!IMPORTANT]
   >
   >在觸發促銷活動智慧清單中使用布林欄位時，您必須明確將其設為「false」，以便欄位在促銷活動執行期間正確評估。

1. 按一下下拉式清單，然後選擇運運算元。

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >紅色曲線表示錯誤或遺失資訊。 如果未更正，此行銷活動將會無效且無法執行。

   >[!TIP]
   >
   >在同時具有觸發器和篩選器的Smart Campaign中，觸發器位於頂端，觸發時，只有符合篩選條件的人員才會通過流程。

1. 定義觸發器。

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >使用多個觸發程式時，如果啟動其中一個&#x200B;_任一_&#x200B;觸發程式，則人員會通過流程。

若要對一組人員同時執行行銷活動，瞭解如何[定義Smart Campaign的智慧清單 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}。

>[!MORELIKETHIS]
>
>[將流程步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
