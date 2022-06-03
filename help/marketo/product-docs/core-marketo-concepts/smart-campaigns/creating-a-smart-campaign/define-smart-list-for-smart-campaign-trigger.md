---
unique-page-id: 1146942
description: 定義智慧市場活動的智慧清單 |觸發器 — Marketo文檔 — 產品文檔
title: 定義智慧市場活動的智慧清單 |觸發器
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 定義智慧市場活動的智慧清單 |觸發器 {#define-smart-list-for-smart-campaign-trigger}

通過添加觸發器，根據即時事件一次在一個人上運行智慧市場活動。

1. 在您的智慧市場活動中，按一下 **智慧清單** 頁籤。

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. 搜索觸發器，然後將觸發器拖放到畫布。

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >具有觸發器的智慧市場活動 **觸發器** 的子菜單。 它根據觸發的事件和任何附加篩選器一次在一個人上運行。

   >[!IMPORTANT]
   >
   >在觸發市場活動智慧清單中使用布爾欄位時，必須將其顯式設定為「false」，以便該欄位在執行市場活動期間能夠正確計算。

1. 按一下下拉框並選擇運算子。

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >紅色曲線表示錯誤或缺少資訊。 如果未更正，市場活動將無效且不會運行。

   >[!TIP]
   >
   >在同時具有觸發器和篩選器的智慧市場活動中，觸發器會在頂部，當觸發時，只有滿足篩選條件的人才會通過流。

1. 定義觸發器。

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >在多個觸發器下，如果 **任意** 觸發器之一被激活。

要同時在一組人員上運行該活動，請學習如何 [定義智慧市場活動的智慧清單 |批處理](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)。

>[!MORELIKETHIS]
>
>[向智慧市場活動添加流步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
