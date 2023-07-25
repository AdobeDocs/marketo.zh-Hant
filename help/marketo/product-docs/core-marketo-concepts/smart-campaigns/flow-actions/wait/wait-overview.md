---
unique-page-id: 1146950
description: 等待 — Marketo檔案 — 產品檔案
title: 等待
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# 等待 {#wait}

## 概觀 {#overview}

使用工具暫停智慧型行銷活動流程中的人員 **等待步驟**.

![](assets/wait-overview.png)

請注意您如何輸入「4小時」之類的自然語言。 執行 **not**&#x200B;但是，請以縮寫表示（即4小時）。 智慧型行銷活動仍會執行，但會忽略等待步驟。

>[!CAUTION]
>
>變更等待步驟的持續時間不會影響已進入該步驟的人。 例如：您有一個等候步驟5天，有人進入，然後您將等候步驟變更為7天 — 該人仍然只會等候原來的5天，才會前進到下一個流程步驟。

>[!TIP]
>
>如果您已有人員處於等待步驟，而您不希望他們在等待期間結束後前進，請插入 [從流量中移除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) 在等待步驟之後。 使用指定要移除的人員 [新增選擇](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) 選項。

## 使用情況 {#usage}

有三種主要方法可使用等待流程步驟：

1. [在等待流程步驟中使用持續時間](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流程步驟中使用日期Token](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
