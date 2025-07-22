---
unique-page-id: 2360401
description: 使用Program Analyzer比較管道成效 — Marketo檔案 — 產品檔案
title: 使用Program Analyzer比較管道成效
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 比較管道效益與[!UICONTROL Program Analyzer] {#compare-channel-effectiveness-with-the-program-analyzer}

使用[!UICONTROL Program Analyzer]來比較管道成本、成員贏取、管道、收入等等，以找出您最有效且最無效的管道。

>[!PREREQUISITES]
>
>[建立[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 在&#x200B;**[!UICONTROL Analytics]**&#x200B;我的Marketo **中按一下**。

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 選取您的程式分析器。

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 將檢視變更為&#x200B;**[!UICONTROL By Channel]**。

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 使用&#x200B;**[!UICONTROL X Axis]**&#x200B;下拉式清單選擇水平軸的量度。 讓我們從&#x200B;**[!UICONTROL Program Cost]**&#x200B;開始。

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. 使用&#x200B;**[!UICONTROL Y Axis]**&#x200B;下拉式清單選擇垂直軸的量度。 在這裡，我們將使用&#x200B;**[!UICONTROL (FT) Pipeline Created]**。

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >您可在程式分析器中選擇的許多量度，都適用於首次接觸(FT)和多點接觸(MT)計算。 瞭解FT和MT歸因[之間的](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)差異很重要。

1. 使用&#x200B;**[!UICONTROL Y Axis]**&#x200B;下拉式清單選擇&#x200B;**[!UICONTROL (MT) Pipeline Created]**。

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   在此多點接觸歸因檢視中，我們發現網路研討會管道對建立的管道影響較大，且成本較Tradeshow和Online Advertising管道低。

   現在，再新增兩個維度吧！

1. 使用&#x200B;**[!UICONTROL Bubble Size]**&#x200B;下拉式清單來選取其他量值，例如&#x200B;**[!UICONTROL New Names]**。

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. 觀看圖表如何變更。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   我們看到網路研討會頻道縮減，測量方式為&#x200B;**[!UICONTROL New Names]**。 我們可以得出結論，雖然此組織擁有許多成員，但在創造新銷售機會方面不如貿易展覽頻道有效。

1. 最後，使用顏色下拉式清單來新增第四個維度。 讓我們選取&#x200B;**[!UICONTROL (FT) Revenue Won]**。

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. 觀察圖形中的色彩變化。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   從顏色中，我們瞭解到，貿易展覽管道（最環保的泡泡）影響了透過首次接觸歸因衡量的最大收入。

1. 現在，如果我們將色彩量度變更為&#x200B;**[!UICONTROL (MT) Revenue Won]**，我們會發現線上Advertising頻道（現在最環保）在一段時間內所影響的收入&#x200B;_超過網路研討會及商展頻道。_

   ![](assets/image2014-9-17-18-3a41-3a40.png)

在我們的範例中，在測量由首次接觸建立的配管時，貿易展覽管道是最昂貴（最靠右）和最成功（Y軸最高）的管道。 現在，讓我們考慮每個頻道中透過多重接觸歸因所建立的管道。

>[!TIP]
>
>這些步驟中的範例會根據建立的管道來測量成效。 使用[!UICONTROL Y Axis]下拉式清單來選取其他測量管道效益的方式，例如[!UICONTROL New Names]、[!UICONTROL Members]、[!UICONTROL Cost per Success]等。

>[!MORELIKETHIS]
>
>* [透過[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)探索方案和管道詳細資料
>* [比較方案效果與[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
