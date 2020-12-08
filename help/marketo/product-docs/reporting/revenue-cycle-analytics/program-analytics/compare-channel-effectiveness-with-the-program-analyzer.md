---
unique-page-id: 2360401
description: 比較渠道有效性與計劃分析器——行銷人員文檔——產品文檔
title: 比較渠道有效性與計劃分析器
translation-type: tm+mt
source-git-commit: f74d028e491aa70913fbe5cf14e536e50dbee32b
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# 比較渠道有效性與計劃分析器 {#compare-channel-effectiveness-with-the-program-analyzer}

使用Program Analyzer比較渠道成本、成員獲取、渠道、收入等，以識別最有效、最不有效的渠道。

>[!NOTE]
>
>**必要條件**
>
>* [建立程式分析器](create-a-program-analyzer.md)


1. 按一下「 **我的** Marketo **」中的Analytics。**

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 選擇您的 **Program Analyzer。**

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 將「檢視」變更 **為** 「 **By Channel**」。

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 使用 **X軸下拉式** ，選擇水準軸的量度。 讓我們從計畫成 **本開始**。

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. 使用「Y軸」下拉式清單來選擇垂直軸的量度。 在這裡，我們將介紹( **FT)Pipeline Created**。

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >您可在程式分析器中選擇的許多度量都可搭配首次接觸(FT)和多點接觸(MT)計算使用。 瞭解FT和MT歸因 [的差異很重要](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)。

1. 使用「 **Y軸** 」(Y Axis **)下拉式選**&#x200B;擇「建立的(MT)管線」(Pipeline Created)。

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   在此多點觸控歸因檢視中，我們發現網路研討會通路對建立的通路有更大的影響力，而且比商展和線上廣告通路的成本更低。

   現在，我們再添加兩個維度！

1. 使用「 **泡泡大小** 」(Bubble Size **)下拉式清單來選取其他測量，例如「**&#x200B;新名稱」(New Names)。

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. 觀看圖形的變更。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   我們看到網路研討會頻道會縮小，由「新名稱」 **測量**。 我們可以得出結論，雖然它擁有許多會員，但在創造新客源方面，它比貿易展渠道的效率更低。

1. 最後，使用「顏色」下拉式清單來新增第四個維度。 讓我們選 **擇(FT)Revenue** **Won**。

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. 觀看圖形中的顏色變化。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   從顏色上，我們瞭解到，以首次接觸歸因衡量，最綠色的泡沫——貿易展渠道，對贏得的最大收入產生了影響。

1. 現在，如果我們將「顏色」量度變更為「 **(MT)Revenue Won**」（贏取收入），我們會發現線上廣告頻道（現在最綠色）在一段時間內的影響比網路研討會和貿易展會頻道更大。

   ![](assets/image2014-9-17-18-3a41-3a40.png)

在我們的範例中，我們看到商展頻道在測量首次接觸所建立的管道時，既是最昂貴（最靠右），也是最成功（Y軸最高）。 現在，讓我們考慮一下透過多點觸控歸因來測量每個管道的管道。

>[!TIP]
>
>這些步驟中的範例會根據建立的管線來評估效能。 使用Y軸下拉式清單選擇其他衡量渠道成效的方式，例如新名稱、成員、每次成功的成本等。

>[!NOTE]
>
>**相關文章**
>
>* [使用Program Analyzer瞭解計畫和渠道詳細資訊](explore-program-and-channel-details-with-the-program-analyzer.md)
>* [比較方案分析器與方案有效性](compare-program-effectiveness-with-the-program-analyzer.md)

>



>[!NOTE]
>
>進一步瞭解 [Revenue Cycle Explorer中的進階分析](http://docs.marketo.com/display/docs/revenue+cycle+analytics)。
