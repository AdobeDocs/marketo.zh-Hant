---
unique-page-id: 2360403
description: 將計畫有效性與計劃分析器——行銷人員文檔——產品文檔進行比較
title: 比較方案分析器與方案有效性
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---


# 將程式有效性與程式分析器進行比較{#compare-program-effectiveness-with-the-program-analyzer}

使用Program Analyzer通過比較方案成本、成員獲取、渠道和收入來識別最有效、最不有效的方案。

>[!PREREQUISITES]
>
>[建立程式分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 按一下「**Analytics**」。

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 選擇您的程式分析器。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 將「檢視」變更為「依方案」。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. 使用「渠道篩選」將檢視範圍縮小為一或兩個渠道。 目前，我們將檢視商展頻道中的計畫。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >將程式篩選為僅一個頻道的快速方式是選取「檢視&#x200B;**** > **依頻道**」，按一下該頻道的泡泡，然後在快顯對話方塊中按一下頻道名稱。

1. 使用「X軸」下拉式清單來選擇水準軸的量度。 我們從計畫成本開始。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 使用「Y軸」下拉式清單來選擇垂直軸的量度。 讓我們選擇「新名稱」，以查找擅長捕獲新銷售機會的程式。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. 開啟滑桿以放大。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >您也可以嘗試從線性變更為對數比例，或從線性變為對數比例，以改善檢視效果。 使用頂部的&#x200B;**Scale**&#x200B;菜單。

1. 探索產生的圖形。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   在我們的例子中，我們瞭解到摺紙展比該頻道的其他節目要好得多，在捕捉新名字時要付出中等代價。 但這並不是全部。 我們將新增兩個量度，以進一步瞭解。

1. 使用「泡泡大小」下拉式清單，選擇要依泡泡大小比較的量度。 我們將以(FT)贏取收入為例。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >您可在程式分析器中選擇的許多度量都可搭配首次接觸(FT)和多點接觸(MT)計算使用。 請務必瞭解FT和MT歸因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)之間的[差異。

1. 觀察圖形中泡泡的變化大小。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   通過添加&#x200B;**(FT)Revenue Won**，我們很快地看到，雖然摺紙博覽會獲得了許多新的品牌，但它帶來的收入相對較少。 此外，我們也看到Paper Fest 12節的名氣越來越少，但名氣也越來越好，因為它影響到贏取的收入（泡泡越大）。

1. 使用「顏色」下拉式清單新增第四個量度。 我們將看(FT)投資收益。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. 觀看圖形中的顏色變化。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

我們看到，Paper Fest 12節不僅會影響更多收入（更大的泡沫），而且儘管其節目成本相對較高（在極右側），但在商展頻道的所有節目中，其投資報酬率（最環保的泡沫）最高。

>[!TIP]
>
>您可以快速比較一個頻道和另一個頻道的節目。 只需使用視窗頂端的&#x200B;**頻道篩選器**&#x200B;即可新增更多頻道。

>[!MORELIKETHIS]
>
>* [使用Program Analyzer瞭解計畫和渠道詳細資訊](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [比較渠道有效性與計劃分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)

