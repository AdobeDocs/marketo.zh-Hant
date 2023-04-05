---
unique-page-id: 1146942
description: 定義智慧促銷活動的智慧清單 |觸發器 — Marketo檔案 — 產品檔案
title: 定義智慧促銷活動的智慧清單 |觸發
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: 56d3d05d5462c79f32f507655266e3bfa0cc6846
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# 定義智慧促銷活動的智慧清單 |觸發 {#define-smart-list-for-smart-campaign-trigger}

透過新增觸發器，讓智慧型促銷活動根據即時事件一次在一個人上執行。

1. 在您的智慧行銷活動中，按一下 **智慧清單** 標籤。

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. 搜尋所需觸發器，並將其拖放至畫布。

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >具有觸發器的智慧型行銷活動會在 **觸發** 模式。 它會根據觸發的事件和任何其他篩選器，一次在一個人上執行。

   >[!IMPORTANT]
   >
   >在觸發促銷活動智慧清單中使用布林欄位時，您必須明確將其設為&#39;false&#39;，讓欄位在執行促銷活動期間能正確評估。

1. 按一下下拉式清單，然後選擇運算子。

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >紅曲線表示錯誤或缺少資訊。 若未更正，則促銷活動將無效，且不會執行。

   >[!TIP]
   >
   >在同時具有觸發器和篩選器的智慧型行銷活動中，觸發器會進入頂端，而觸發時，只有符合篩選條件的人才會經過流程。

1. 定義觸發器。

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >若有多個觸發器，若 **任何** 其中一個觸發器被激活。

若要同時在一組人員上執行行銷活動，請了解如何 [定義智慧促銷活動的智慧清單 |批](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[新增流量步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
