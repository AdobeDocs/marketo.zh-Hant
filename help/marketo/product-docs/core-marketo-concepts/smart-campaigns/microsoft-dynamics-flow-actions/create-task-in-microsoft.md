---
unique-page-id: 37356429
description: 在Microsoft中建立任務 — Marketo檔案 — 產品檔案
title: 在Microsoft中建立任務
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 在Microsoft中建立任務 {#create-task-in-microsoft}

身為行銷人員，您擁有可協助銷售完成交易的資訊。 您可以建立任務，讓他們知道應該做什麼，以及何時應該做。

在Microsoft中建立任務會在中與人員（潛在客戶或連絡人）相關的活動下建立任務。 [!DNL Microsoft].

>[!NOTE]
>
>此流程步驟將 _只有在搭配觸發器使用時才有效_，而非篩選器。

根據預設，流程步驟將如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>Marketo同步使用者建立任務時， **[!UICONTROL 到期時間]** 是要於中建立之任務的必填欄位 [!DNL Microsoft]. 如果未輸入值，Marketo預設會輸入五天。

自訂所有欄位，以您想要的方式建立任務。

![](assets/msd2.png)

>[!NOTE]
>
>在「流程動作」中為工作指定的「狀態」欄位會更新中的「狀態原因」欄位。 [!DNL Microsoft].

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`， `{{company.tokens}}`， `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **[!UICONTROL 主旨]** 和 **[!UICONTROL 說明]**. 另請參閱 [流程步驟的權杖](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} 以取得更多詳細資料。
