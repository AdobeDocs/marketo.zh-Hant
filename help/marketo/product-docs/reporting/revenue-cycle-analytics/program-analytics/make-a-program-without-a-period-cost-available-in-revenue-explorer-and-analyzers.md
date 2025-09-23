---
unique-page-id: 2360389
description: 在「收入總管」與「分析器 — Marketo檔案 — 產品檔案」中，提供不含期間成本的方案
title: 讓營收總管及分析工具可以包含沒有期間成本的方案
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 10%

---

# 讓營收總管及分析工具可以包含沒有期間成本的方案 {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

方案期間成本可讓您定義方案的「金額」和「時間」。 這會顯示在Revenue Cycle Explorer和[分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md)中。

>[!NOTE]
>
>**需要管理員許可權**

某些計畫即使沒有期間成本，也可能需要包括在內。 雖然您可以輸入0作為期間成本，但我們已讓納入這些計畫變得更容易。

>[!NOTE]
>
>「方案分析器」會依期間成本儲存方案成功。 如果沒有可用的期間成本，無論方案的分析行為為何，都不會顯示方案成功。 如果設定分析行為，將顯示機會量度的資料（管道機會、贏取收入等）。

1. 在[!UICONTROL Admin]區段下，按一下&#x200B;**[!UICONTROL Tags]**。

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. 展開頻道，然後按兩下您選取的頻道。

   >[!NOTE]
   >
   >使用此管道的所有程式（無論期間成本為何）都將可供收入總管和分析器使用。 此變更將於次日生效。

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. 將[!UICONTROL Analytics Behavior]變更為&#x200B;**包含**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>您注意到操作選項嗎？ 反之亦然。 無論期間成本為何，都會排除這些程式。

做得好！ 現在，使用修改後管道的任何計畫都將包含在收入總管和分析器中，而無需期間成本。

>[!MORELIKETHIS]
>
>[覆寫程式層級](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)的分析行為
