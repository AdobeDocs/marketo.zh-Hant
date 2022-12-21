---
unique-page-id: 2360401
description: 與Program Analyzer - Marketo檔案 — 產品檔案比較管道效益
title: 比較渠道有效性與程式分析器
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 比較渠道有效性與程式分析器 {#compare-channel-effectiveness-with-the-program-analyzer}

使用Program Analyzer來比較渠道成本、成員獲取、管道、收入等，以確定最有效和最低效的渠道。

>[!PREREQUISITES]
>
>[建立程式分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 按一下 **Analytics** in **我的Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 選取 **程式分析器**.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 將檢視變更為 **依管道**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 使用 **X軸** 下拉式清單，選擇水準軸的量度。 讓我們從 **計畫成本**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. 使用「Y軸」下拉式清單來選擇垂直軸的量度。 來，我們一起去 **(FT)管道已建立**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >您可在程式分析器中選擇的許多量度都提供首次接觸(FT)和多次接觸(MT)計算。 了解 [FT和MT歸因的差異](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. 使用 **Y軸** 要選擇的下拉式清單 **(MT)管道已建立**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   透過此多點接觸歸因檢視，我們發現網路研討會管道對建立管道的影響力較大，且成本比貿易展會和線上廣告管道低。

   現在，再新增兩個維度！

1. 使用 **氣泡大小** 下拉式清單以選取其他測量，例如 **新名稱**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. 觀看圖表的變更。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   我們發現，網路研討會頻道收縮，如 **新名稱**. 我們可以得出結論，儘管它有很多會員，但在創造新銷售機會方面，它不如貿易展渠道有效。

1. 最後，使用「顏色」下拉式清單來新增第四個維度。 我們選取 **(FT)收入韓元**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. 觀看圖表中的顏色變更。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   從顏色中，我們了解到，最綠色的泡沫 — 貿易展渠道，對贏得的最大收入產生了影響，這是由首次接觸歸因所衡量的。

1. 現在，如果我們將「顏色」量度變更為 **(MT)收入成本**，我們發現線上廣告管道（現為最綠色的管道）隨著時間的推移，對收入的影響比網路研討會和貿易展管道更多。

   ![](assets/image2014-9-17-18-3a41-3a40.png)

在我們的範例中，我們發現貿易展廳管道在測量由首次接觸建立的管道時，既最昂貴（最靠右），也最成功（Y軸最高）。 現在，讓我們考慮由多點接觸歸因所測量的每個管道管道。

>[!TIP]
>
>這些步驟中的範例會根據建立的管道來評估成效。 使用「Y軸」(Y Axis)下拉清單選擇其他方法來測量通道有效性，如「新名稱」(New Name)、「成員」(Members)、「每次成功的成本」(Cost per Success)等。

>[!MORELIKETHIS]
>
>* [使用Program Analyzer探索Program &amp; Channel詳細資訊](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [與程式分析器比較程式效果](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)

