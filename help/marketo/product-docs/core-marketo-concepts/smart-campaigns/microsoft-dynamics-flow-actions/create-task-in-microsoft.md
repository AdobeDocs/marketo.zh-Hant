---
unique-page-id: 37356429
description: 在Microsoft中建立任務 — Marketo檔案 — 產品檔案
title: 在Microsoft中建立任務
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 在Microsoft中建立任務 {#create-task-in-microsoft}

身為行銷人員，您擁有可協助銷售完成交易的資訊。 您可以建立任務，讓他們知道應該做什麼，以及何時應該做。

在Microsoft中建立任務會在[!DNL Microsoft]中與人員（潛在客戶或連絡人）相關的活動下建立任務。

>[!NOTE]
>
>此流程步驟&#x200B;_只有在您的智慧行銷活動中與觸發程式_&#x200B;搭配使用時才有效，不會與篩選器搭配使用。

根據預設，流程步驟將如下所示：

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>當Marketo同步使用者建立任務時，**[!UICONTROL 在]**&#x200B;到期是將在[!DNL Microsoft]中建立任務的必要欄位。 如果未輸入值，Marketo預設會輸入五天。

自訂所有欄位，以您想要的方式建立任務。

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>在「流程動作」中為工作指定的「狀態」欄位會更新[!DNL Microsoft]中的「狀態原因」欄位。

>[!TIP]
>
>您可以在&#x200B;**[!UICONTROL 主旨]**&#x200B;和&#x200B;**[!UICONTROL 描述]**&#x200B;中使用`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`和`{{system.tokens}}`。 如需詳細資訊，請參閱流程步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}的[權杖。
