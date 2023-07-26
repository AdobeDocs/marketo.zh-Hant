---
unique-page-id: 37356429
description: 在Microsoft中建立任務 — Marketo檔案 — 產品檔案
title: 在Microsoft中建立任務
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 在Microsoft中建立任務 {#create-task-in-microsoft}

身為行銷人員，您擁有可協助銷售完成交易的資訊。 您可以建立任務，讓他們知道應該做什麼，以及何時應該做。

在Microsoft中建立任務會在Microsoft中與人員（潛在客戶或聯絡人）相關的活動下建立任務。

>[!NOTE]
>
>此流程步驟將 **只有在搭配觸發器使用時才有效**，而非篩選器。

根據預設，流程步驟將如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>Marketo同步使用者建立任務時， **到期時間** 是要在Microsoft中建立之任務的必填欄位。 如果未輸入值，Marketo預設會輸入五天。

自訂所有欄位，以您想要的方式建立任務。

![](assets/msd2.png)

>[!NOTE]
>
>在「流程動作」中為任務指定的「狀態」欄位會更新Microsoft中的「狀態原因」欄位。

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`， `{{company.tokens}}`， `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **主旨** 和 **說明**. 另請參閱 [流程步驟的權杖](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) 以取得更多詳細資料。
