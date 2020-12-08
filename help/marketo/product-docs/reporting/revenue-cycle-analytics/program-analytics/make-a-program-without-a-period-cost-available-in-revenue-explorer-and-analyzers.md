---
unique-page-id: 2360389
description: 在Revenue Explorer和Analyzers - Marketo Docs - Product Documentation中提供不含期間成本的計畫
title: 在收入瀏覽器和分析器中提供不含期間成本的方案
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# 在收入瀏覽器和分析器中提供不含期間成本的方案 {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

方案期間成本允許您為方案定義「金額」和「時間」。 這會顯示在收入 [週期瀏覽器](http://docs.marketo.com/display/docs/revenue+cycle+analytics) 和分 [析器中](../../../../product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md)。

>[!NOTE]
>
>**需要管理員權限**

有些方案即使沒有期限成本，也可能需要納入。 雖然您可以在期間成本中輸入0，但我們已更輕鬆地納入這些方案。

>[!NOTE]
>
>Program Analyzer將按期間成本計算程式成功率。 如果沒有期間成本，則不會顯示「方案成功」，不論方案的分析行為為何。 如果設定了分析行為，則會針對機會度量（管道商機、贏取收入等）顯示資料。

1. 在「管理」區段下，按一下「標籤」。

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. 展開您的渠道，然後按兩下您選擇的渠道。

   >[!NOTE]
   >
   >**提醒**
   >
   >使用此渠道的所有方案（不論期間成本）都將可供收入瀏覽器和分析器使用。 此變更將於次日生效。

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. 將「分析行為」變更為「包含」，然後按一下「儲存」。

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>您注意到「操作」選項了嗎？ 這恰恰相反。 不論期間成本為何，都會排除這些方案。

幹得好！ 現在，任何使用已修改渠道的程式都將包含在收入瀏覽器和分析器中，而不需要期間成本。

>[!NOTE]
>
>**相關文章**
>
>* [在方案層級覆寫分析行為](override-analytics-behavior-at-the-program-level.md)

>



