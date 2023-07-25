---
unique-page-id: 1147001
description: 使用標準智慧清單規則邏輯 — Marketo檔案 — 產品檔案
title: 使用標準智慧清單規則邏輯
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用標準智慧清單規則邏輯 {#using-standard-smart-list-rule-logic}

您在建立行銷活動智慧清單時，可能會注意到「使用篩選器」選項。 此設定可讓您決定是否需要使用AND或OR運運算元評估篩選器。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>變更智慧清單規則邏輯僅適用於篩選器， **not** 觸發器。

系統會一律將觸發器評估為「或」，即使上述設定設為「全部」亦然。  範例如下：

![](assets/image2014-9-22-14-3a12-3a57.png)

上述智慧清單的字詞如下：

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

所以，如果有人填寫表格 **或** 造訪頁面時，行銷活動會根據以下條件評估該人員： **全部** 或 **任何** 後續篩選器的預設值（視使用的設定而定）。

>[!MORELIKETHIS]
>
>[使用進階智慧列示規則邏輯](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
