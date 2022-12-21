---
unique-page-id: 1146950
description: 等待 — Marketo檔案 — 產品檔案
title: 等待
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# 等待 {#wait}

## 總覽 {#overview}

使用可用功能，將人員暫停在智慧型行銷活動流程中 **等待步驟**.

![](assets/wait-overview.png)

請注意，如何輸入「4小時」之類的自然語言。 做 **not**&#x200B;但是，縮略了字詞（即4小時）。 智慧型行銷活動仍會執行，但會忽略等待步驟。

>[!CAUTION]
>
>更改等待步驟的持續時間不會影響已輸入步驟的人員。 例如：您有5天的等待步驟，有人進入，然後您將等待步驟變更為7天 — 該人仍只等待原始的5天，然後才進入下一個流步驟。

>[!TIP]
>
>如果某個人已在等待步驟中，並且不希望他們在等待期間結束後繼續，請插入 [從流中刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) 在等待步驟之後。 指定您要移除的對象，方法是使用 [新增選擇](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) 選項。

## 使用情況 {#usage}

有三種主要方式可使用等待流程步驟：

1. [在等待流程步驟中使用持續時間](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流程步驟中使用日期代號](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
