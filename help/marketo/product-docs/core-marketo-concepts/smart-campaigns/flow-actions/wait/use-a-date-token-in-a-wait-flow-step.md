---
unique-page-id: 1146997
description: 瞭解如何在等待流程步驟中使用日期代號。 等到權杖的動態日期再繼續。
title: 在等待流程步驟中使用日期權杖
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/b59TeCenvUee5sOw3O4ggclGMEdkhX3RlC31DWh5d08
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 8%

---

# 在等待流程步驟中使用日期權杖 {#use-a-date-token-in-a-wait-flow-step}

您可以使用等待流程步驟來暫停使用者通過Smart Campaign的歷程，直到使用日期權杖的特定日期為止。 您也可以將結束日期修改幾天。

>[!NOTE]
>
>這僅適用於觸發行銷活動。 您無法在批次行銷活動中使用此功能。

1. 在您的Smart Campaign **[!UICONTROL Flow]**&#x200B;標籤中，拖曳至&#x200B;**[!UICONTROL Wait]**&#x200B;流程步驟上。

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. 按一下齒輪圖示。

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. 從&#x200B;**[!UICONTROL Type]**&#x200B;下拉式清單中選取&#x200B;**[!UICONTROL Date Token]**。

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. 選擇[!UICONTROL Date token]以指定等待步驟的結束時間：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. 若要等到目前或下一個日曆年度中出現的日期的下一個週年紀念日，請核取方塊。

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >在參考過去日期（例如生日或合約開始日期）的日期權杖上使用此選項。

1. 或者，您可以依指定天數修改結束日期。

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >您也可以使用代表整數欄位的`{{lead.`或`{{company.`權杖或數字型別的`{{my.`權杖來指定天數。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流程步驟中使用持續時間](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
