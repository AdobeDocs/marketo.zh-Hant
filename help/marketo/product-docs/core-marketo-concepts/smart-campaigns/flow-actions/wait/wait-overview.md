---
unique-page-id: 1146950
description: 等待-Marketo文檔——產品文檔
title: 等待
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 等待{#wait}

## 概述{#overview}

使用方便的&#x200B;**等待步驟**&#x200B;暫停智慧型促銷活動流程中的人員。

![](assets/wait-overview.png)

請注意，您如何輸入自然語言，例如「4小時」。 不過，請&#x200B;**not**&#x200B;縮寫這些字詞（即4小時）。 智慧型促銷活動仍會執行，但會忽略等待步驟。

>[!CAUTION]
>
>更改等待步驟的持續時間不會影響已輸入步驟的人員。 例如：您有5天的等待步驟，某人進入該步驟，然後您將等待步驟更改為7天——該人仍然只等待原始的5天，然後才進入下一個流程步驟。

>[!TIP]
>
>如果有人已在等待步驟中，而不希望他們在等待期間結束後繼續，請在等待步驟後插入[從流](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)中刪除。 使用[add choice](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md)選項指定要移除的人。

## 用法{#usage}

使用等待流程步驟有三種主要方式：

1. [在等待流程步驟中使用持續時間](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流程步驟中使用日期Token](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
