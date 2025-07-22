---
unique-page-id: 2360403
description: 使用計劃分析器比較計畫成效 — Marketo檔案 — 產品檔案
title: 使用方案分析器比較方案效能
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 與[!UICONTROL Program Analyzer]比較方案成效 {#compare-program-effectiveness-with-the-program-analyzer}

使用[!UICONTROL Program Analyzer]來比較方案成本、成員贏取、管道和收入，以識別您最有效且最無效的方案。

>[!PREREQUISITES]
>
>[建立[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 按一下「**[!UICONTROL Analytics]**」。

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 選取您的程式分析器。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 將檢視變更為&#x200B;**[!UICONTROL By Program]**。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. 使用&#x200B;**[!UICONTROL Channel Filter]**&#x200B;將檢視縮小至一或兩個色版。 目前，我們將在&#x200B;**[!UICONTROL Tradeshow]**&#x200B;頻道中檢視計畫。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >若要將節目篩選為只有一個頻道，快速的方法是選取&#x200B;**[!UICONTROL View]** > **[!UICONTROL By Channel]**，按一下該頻道的泡泡，然後在快顯對話方塊中按一下頻道名稱。

1. 使用&#x200B;**[!UICONTROL X Axis]**&#x200B;下拉式清單選擇水平軸的量度。 我們將從&#x200B;**[!UICONTROL Program Cost]**&#x200B;開始。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 使用&#x200B;**[!UICONTROL Y Axis]**&#x200B;下拉式清單選擇垂直軸的量度。 讓我們選擇&#x200B;**[!UICONTROL New Names]**&#x200B;來尋找擅長擷取新潛在客戶的程式。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. 開啟滑桿以放大。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >您也可以嘗試透過將線性縮放變更為對數縮放來改善檢視，反之亦然。 使用頂端的&#x200B;**[!UICONTROL Scale]**&#x200B;功能表。

1. 探索產生的圖表。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   在我們的範例中，我們瞭解[!DNL Origami Expo]在擷取新名稱方面遠遠優於該頻道中的所有其他程式，而且成本適中。 但這還不是故事的全部。 我們將新增兩個量度，以更深入地瞭解。

1. 使用&#x200B;**[!UICONTROL Bubble Size]**&#x200B;下拉式清單選擇要以泡泡大小比較的量度。 我們將選擇&#x200B;**[!UICONTROL (FT) Revenue Won]**&#x200B;作為範例。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >您可在程式分析器中選擇的許多量度，都適用於首次接觸(FT)和多點接觸(MT)計算。 瞭解FT和MT歸因[之間的](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)差異很重要。

1. 觀察圖表中的泡泡大小變化。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   新增&#x200B;**[!UICONTROL (FT) Revenue Won]**&#x200B;後，我們很快發現[!DNL Origami Expo]雖然獲得許多新名稱，但產生的收入卻相對較少。 此外，我們看到[!DNL Paper Fest 12]程式名稱越來越少，但名稱越來越好，因為這會影響贏得的更多收入（更大的泡泡）。

1. 使用色彩下拉式清單來新增第四個量度。 我們將檢視&#x200B;**[!UICONTROL (FT) Revenue to Investment]**。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. 觀察圖形中的色彩變化。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

我們看到[!DNL Paper Fest 12]方案不僅會影響更多收入（更大的泡泡），儘管其方案成本相對較高（位於最右邊），但在[!UICONTROL Tradeshow]頻道中的所有方案中，其投資報酬率（最環保的泡泡）最佳。

>[!TIP]
>
>您可以快速比較一個管道中的方案與另一個管道中的方案。 只要使用視窗頂端的&#x200B;**頻道篩選器**&#x200B;來新增更多頻道即可。

>[!MORELIKETHIS]
>
>* [透過[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)探索方案和管道詳細資料
>* [比較管道效益與[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
