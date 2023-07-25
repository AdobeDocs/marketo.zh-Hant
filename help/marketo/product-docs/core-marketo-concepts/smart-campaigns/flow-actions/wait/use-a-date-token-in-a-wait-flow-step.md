---
unique-page-id: 1146997
description: 在等待流程步驟中使用日期權杖 — Marketo檔案 — 產品檔案
title: 在等待流程步驟中使用日期Token
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 在等待流程步驟中使用日期Token {#use-a-date-token-in-a-wait-flow-step}

您可以使用等待流程步驟來暫停個人通過智慧行銷活動的歷程，直到使用日期權杖的特定日期為止。 您也可以將結束日期修改一些天數。

>[!NOTE]
>
>這僅適用於觸發行銷活動。 您無法在批次行銷活動中使用此功能。

1. 在您的智慧行銷活動中 **流量** 標籤，拖曳至 **等待** 流程步驟。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 按一下右側的齒輪圖示。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 從 **型別** 下拉式清單，選取 **日期Token**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 選擇日期權杖，以指定等待步驟的結束時間：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 若要等到目前或下一個日曆年度中出現的日期的下一個週年紀念日，請核取方塊。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >在參考過去日期（例如生日或合約開始日期）的日期Token上使用此選項。

1. 或者，您可以依指定天數來修改結束日期。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >您也可以使用指定天數 `{{lead.` 或 `{{company.` 代表整數欄位的權杖，或 `{{my.` 數字型別的Token。

1. 按一下 **儲存**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流程步驟中使用持續時間](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
