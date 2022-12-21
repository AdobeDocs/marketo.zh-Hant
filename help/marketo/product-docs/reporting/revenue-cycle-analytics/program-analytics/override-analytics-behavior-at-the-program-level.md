---
unique-page-id: 2360421
description: 覆寫方案層級的Analytics行為 — Marketo檔案 — 產品檔案
title: 覆寫方案層級的Analytics行為
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 覆寫方案層級的Analytics行為 {#override-analytics-behavior-at-the-program-level}

您可以設定 [管道上管理層級的analytics行為](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md) 但您也可以在方案層級覆寫它。 方法如下：

1. 前往 **行銷活動** 的上界。

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. 尋找並選取您的方案。

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. 在 **設定** 標籤中，將「Analytics行為」拖曳至畫布中。

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. 選取您想要的Analytics行為。

   >[!NOTE]
   >
   >**定義**
   >
   >* **包含**  — 此選項可確保方案可用於收入瀏覽器和分析器中的報告，無論您是否已包括期間成本。
   >* **操作**  — 此選項會導致收入總管或分析器中未顯示方案。


   >[!NOTE]
   >
   >預設行為（如果未套用此設定）是會將程式納入Analytics中 **僅當至少存在一個期間成本時**，即使分配了零美元。

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. 按一下 **儲存**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

幹得好！ 現在您知道如何覆寫方案層級的分析行為。

>[!NOTE]
>
>變更將會影響隔天，且可供使用或從收入總管和分析器中提取。
