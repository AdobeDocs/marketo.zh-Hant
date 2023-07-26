---
unique-page-id: 2360403
description: 使用計劃分析器比較計畫成效 — Marketo檔案 — 產品檔案
title: 使用方案分析器比較方案效能
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 使用方案分析器比較方案效能 {#compare-program-effectiveness-with-the-program-analyzer}

使用Program Analyzer，透過比較方案成本、成員贏取、管道和收入，找出您最有效和最不有效的方案。

>[!PREREQUISITES]
>
>[建立程式分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 按一下 **Analytics**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 選取您的程式分析器。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 將檢視變更為「依計畫」。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. 使用「色版篩選」將檢視縮小至一或兩個色版。 現在，我們將在Tradeshow頻道中檢視計畫。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >若要快速將方案篩選為只有一個管道，請選取 **檢視** > **依頻道**，按一下該管道的泡泡，然後在快顯視窗對話方塊中按一下管道名稱。

1. 使用「X軸」下拉式清單，選擇水平軸的量度。 我們將從計畫成本開始。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 使用「Y軸」下拉式清單，選擇垂直軸的量度。 讓我們選擇「新名稱」來尋找擅長擷取新潛在客戶的程式。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. 開啟滑桿以放大。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >您也可以嘗試透過將線性縮放變更為對數縮放來改善檢視，反之亦然。 使用 **縮放** 功能表頂端。

1. 探索產生的圖表。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   在我們的範例中，我們瞭解到Origami Expo在擷取新名稱方面遠遠勝過該頻道中的所有其他計畫，而且成本適中。 但這還不是故事的全部。 我們將新增兩個量度，以更深入地瞭解。

1. 使用「泡泡大小」下拉式清單，選擇要依泡泡大小比較的量度。 我們將以範例來選擇(FT) Revenue Won。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >您可在程式分析器中選擇的許多量度，都適用於首次接觸(FT)和多點接觸(MT)計算。 瞭解 [FT和MT歸因的差異](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. 觀察圖表中的泡泡大小變化。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   藉由新增 **(FT)贏得的收入**，我們很快發現，雖然摺紙博覽會獲得了許多新名稱，但帶來的收入卻相對較少。 此外，我們看到Paper Fest 12計畫的名稱越來越少，但名稱卻越來越好，因為這會影響更多的收入（更大的泡泡圖）。

1. 使用色彩下拉式清單來新增第四個量度。 我們將審視(FT)投資收入。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. 觀察圖形中的色彩變化。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

我們看到Paper Fest 12方案不僅會影響更多收入（更大的泡泡），儘管方案成本相對較高（位於最右邊），但在商展頻道的所有方案中，它的投資報酬率（最環保的泡泡）是最高的。

>[!TIP]
>
>您可以快速比較一個管道中的方案與另一個管道中的方案。 只要使用 **頻道篩選器** 以新增更多管道。

>[!MORELIKETHIS]
>
>* [使用方案分析器探索方案和管道詳細資訊](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [使用Program Analyzer比較管道成效](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
