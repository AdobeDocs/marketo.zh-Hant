---
unique-page-id: 2360389
description: 在Revenue Explorer和Analyzers - Marketo檔案 — 產品檔案中提供不含期間成本的計畫
title: 在「收入總管」和「分析器」中設定不含期間成本的程式
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 在「收入總管」和「分析器」中設定不含期間成本的程式 {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

方案期間成本允許您定義方案的「金額」和「時間」。 這會顯示在「收入週期總管」和 [分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**需要管理權限**

即使沒有期限費用，也可能需要包括某些計畫。 雖然您可以為期間成本輸入0，但我們使納入這些計畫更為容易。

>[!NOTE]
>
>程式分析器分段程式按期間成本成本成功。 如果沒有可用的期間成本，無論方案的分析行為為何，都不會顯示方案成功。 如果已設定分析行為，則會顯示機會量度（管道機會、贏取收入等）的資料。

1. 在「管理員」區段下，按一下 **標籤**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. 展開「管道」，然後連按兩下您選取的管道。

   >[!NOTE]
   >
   >使用此管道的所有程式（不論期間成本為何）將可供收入總管和分析器使用。 此變更將於次日生效。

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. 將Analytics行為變更為「包含」，然後按一下 **儲存**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>您注意到「操作」選項了嗎？ 這恰恰相反。 它不包括這些方案，而不考慮期間費用。

幹得好！ 現在，使用已修改管道的任何程式都會包含在收入總管和分析器中，而不需要期間成本。

>[!MORELIKETHIS]
>
>[覆寫方案層級的Analytics行為](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
