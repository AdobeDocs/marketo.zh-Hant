---
unique-page-id: 2360421
description: 覆寫方案層級的分析行為——行銷檔案——產品檔案
title: 在方案層級覆寫分析行為
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# 覆寫程式層級{#override-analytics-behavior-at-the-program-level}的分析行為

您可以在管理層級設定[渠道](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md)的分析行為，但您也可以在程式層級覆寫它。 以下是方法：

1. 前往&#x200B;**行銷活動**&#x200B;區域。

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. 尋找並選取您的方案。

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. 在&#x200B;**Setup**&#x200B;標籤下，將Analytics行為拖曳至畫布中。

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. 選取您想要的Analytics行為。

   >[!NOTE]
   >
   >**定義**
   >
   >* **包含** -此選項可確保方案可用於收入瀏覽器和分析器中的報告，無論您是否已包括期間成本。
   >* **Operational**  —— 此選項會導致方案未顯示在收入瀏覽器或分析器中。


   >[!NOTE]
   >
   >預設行為（如果未套用此設定）是只有在至少有一個期間成本&#x200B;**（即使指派零美元）時，才會將程式納入Analytics**。

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2014-9-24-11-3a42-3a6.png)

幹得漂亮！ 現在您知道如何覆寫程式層級的分析行為。

>[!NOTE]
>
>這些變更將會在第二天生效，而且會提供或從收入瀏覽器和分析器中取出。
