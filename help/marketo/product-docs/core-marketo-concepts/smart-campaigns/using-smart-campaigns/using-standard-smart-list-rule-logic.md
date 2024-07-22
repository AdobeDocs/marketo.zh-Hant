---
unique-page-id: 1147001
description: 使用標準智慧清單規則邏輯 — Marketo檔案 — 產品檔案
title: 使用標準智慧清單規則邏輯
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用標準智慧清單規則邏輯 {#using-standard-smart-list-rule-logic}

您在建立Campaign智慧清單時，可能會注意到「使用篩選器」選項。 此設定可讓您決定是否需要使用AND或OR運運算元評估篩選器。

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>變更智慧列示規則邏輯僅適用於篩選器，_不是_&#x200B;觸發器。

系統會一律將觸發器評估為OR，即使上述設定設為ALL亦然。 範例如下：

![](assets/using-standard-smart-list-rule-logic-2.png)

上述智慧清單（以文字表示）：

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page 
AND 
Industry is Energy 
AND 
Country is US 
THEN follow the campaign's flow step(s)
```

因此，如果有人填寫表單&#x200B;_或_&#x200B;造訪該頁面，則行銷活動會根據後續篩選器的&#x200B;_所有_&#x200B;或&#x200B;_任何_ （視使用的設定而定）評估該人。

>[!MORELIKETHIS]
>
>[使用進階智慧清單規則邏輯](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
