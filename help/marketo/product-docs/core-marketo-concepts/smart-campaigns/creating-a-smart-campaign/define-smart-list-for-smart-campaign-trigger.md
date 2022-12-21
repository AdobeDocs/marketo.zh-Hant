---
unique-page-id: 1146942
description: 定義智慧促銷活動的智慧清單 |觸發器 — Marketo檔案 — 產品檔案
title: 定義智慧促銷活動的智慧清單 |觸發
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 定義智慧促銷活動的智慧清單 |觸發 {#define-smart-list-for-smart-campaign-trigger}

透過新增觸發器，根據即時事件，一次在一個人上執行智慧型促銷活動。

1. 在您的智慧型行銷活動中，按一下 **智慧清單** 標籤。

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. 搜尋觸發器，然後將觸發器拖放至畫布。

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >具有觸發器的智慧型行銷活動會在 **觸發** 模式。 它會根據觸發的事件和任何其他篩選器，一次在一個人上執行。

   >[!IMPORTANT]
   >
   >在觸發促銷活動智慧清單中使用布林欄位時，您必須明確將其設為&#39;false&#39;，讓欄位在執行促銷活動期間能正確評估。

1. 按一下下拉式清單，然後選擇運算子。

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >紅曲線表示錯誤或缺少資訊。 若未更正，則促銷活動將無效，且不會執行。

   >[!TIP]
   >
   >在同時具有觸發器和篩選器的智慧型行銷活動中，觸發器會進入頂端，而觸發時，只有符合篩選條件的人才會經過流程。

1. 定義觸發器。

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >若有多個觸發器，若 **任何** 其中一個觸發器被激活。

若要同時在一組人員上執行行銷活動，請了解如何 [定義智慧促銷活動的智慧清單 |批](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[新增流量步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
