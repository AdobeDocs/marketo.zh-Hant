---
unique-page-id: 1147017
description: 瞭解如何在流程步驟中建立Salesforce任務。 當有人進入流程時，為潛在客戶擁有者建立作業。
title: 建立工作
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/RJ5nZrVvURtgXEWWZwL2xXzlYOhWjKGSbX-MFTWCwzg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 126
ht-degree: 3%

---

# 建立工作 {#create-task}

身為行銷人員，您擁有可協助銷售完成交易的資訊。 您可以建立任務，讓他們知道應該做什麼，以及何時應該做。

![](assets/create-task-1.png)

>[!NOTE]
>
>當Marketo Sync使用者建立任務時，**[!UICONTROL Due In]**&#x200B;為要在Salesforce中建立之任務的必要欄位。 如果沒有值，Marketo預設會輸入5天。

根據預設，流程步驟將如下所示：

![](assets/create-task-2.png)

自訂所有欄位，以您想要的方式建立任務。

![](assets/create-task-3.png)

>[!TIP]
>
>您可以在&#x200B;**[!UICONTROL Subject]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;中使用`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`和`{{system.tokens}}`。 如需詳細資訊，請參閱流程步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}的[權杖。
