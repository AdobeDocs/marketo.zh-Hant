---
unique-page-id: 2360421
description: 覆寫方案層級的Analytics行為 — Marketo檔案 — 產品檔案
title: 覆寫方案層級的Analytics行為
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 覆寫方案層級的Analytics行為 {#override-analytics-behavior-at-the-program-level}

您可以設定 [在管道上的管理員層級分析行為](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md) 但您也可以在方案層級覆寫它。 方法如下：

1. 前往 **行銷活動** 區域。

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. 尋找並選取您的程式。

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. 在 **設定** 標籤，將「Analytics行為」拖曳至畫布。

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. 選取您想要的Analytics行為。

   >[!NOTE]
   >
   >**定義**
   >
   >* **包含**  — 此選項將確保程式可用於在收入總管和分析器中報告，無論您是否包含期間成本。
   >* **營運**  — 此選項導致計畫未顯示在收入總管或分析器中。

   >[!NOTE]
   >
   >預設行為（如果未套用此設定）是包含在Analytics中的程式 **僅當至少有一個期間成本時**，即使指派了零美元也一樣。

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. 按一下 **儲存**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

做得很好！ 現在您知道如何在方案層級覆寫分析行為了。

>[!NOTE]
>
>這些變更將在隔天生效，並且可供使用或從收入總管和分析器中提取。
