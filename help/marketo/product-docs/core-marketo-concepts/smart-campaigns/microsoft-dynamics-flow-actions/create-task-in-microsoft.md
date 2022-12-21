---
unique-page-id: 37356429
description: 在Microsoft中建立任務 — Marketo檔案 — 產品檔案
title: 在Microsoft中建立任務
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 在Microsoft中建立任務 {#create-task-in-microsoft}

身為行銷人員，您擁有有助於銷售完成交易的資訊。 您可以建立任務，讓他們知道應該做什麼以及何時應該做什麼。

在Microsoft中建立任務會在Microsoft中與人員（銷售機會或聯絡人）相關的活動下建立任務。

>[!NOTE]
>
>此流程步驟將 **搭配觸發器使用時僅有效**，而非篩選。

依預設，流程步驟如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>Marketo同步用戶建立任務時， **到期日** 是在Microsoft中建立任務的必填欄位。 如果未輸入值，Marketo預設會輸入5天。

自訂所有欄位，以您想要的方式建立任務。

![](assets/msd2.png)

>[!NOTE]
>
>為「流動操作」中的任務指定的欄位「狀態」將更新該欄位：Microsoft中的「狀態原因」。

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **主旨** 和 **說明**. 請參閱 [流程步驟的代號](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) 以取得更多詳細資訊。
