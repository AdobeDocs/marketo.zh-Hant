---
unique-page-id: 1146997
description: 在等候流程步驟中使用日期代號 — Marketo檔案 — 產品檔案
title: 在等待流程步驟中使用日期代號
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 在等待流程步驟中使用日期代號 {#use-a-date-token-in-a-wait-flow-step}

您可以使用「等待流程」步驟，將人員的歷程暫停在智慧型促銷活動中，直到使用日期代號的特定日期為止。 您也可以修改結束日期（天數）。

>[!NOTE]
>
>這僅適用於觸發促銷活動。 您無法在批次促銷活動中使用此功能。

1. 在您的智慧行銷活動中 **流量** 標籤，拖曳至 **等待** 流程步驟。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 按一下右側的齒輪圖示。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 從 **類型** 下拉式清單，選取 **日期代號**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 選擇日期代號，以指定等待步驟應在何時結束：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 要等到當前日曆年或下一個日曆年發生日期的下一個週年，請核取方塊。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >在日期代號中使用此選項，這些代號是指過去的日期，例如生日或合約開始日期。

1. （可選）您可以按指定天數修改結束日期。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >您也可以使用 `{{lead.` 或 `{{company.` 代表整數欄位或 `{{my.` 數字類型的代號。

1. 按一下 **儲存**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流程步驟中使用持續時間](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

