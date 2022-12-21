---
unique-page-id: 1147001
description: 使用標準智慧清單規則邏輯 — Marketo檔案 — 產品檔案
title: 使用標準智慧清單規則邏輯
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用標準智慧清單規則邏輯 {#using-standard-smart-list-rule-logic}

建立促銷活動智慧清單時，您可能已注意到「使用篩選器」選項。 此設定可讓您決定是否需要使用AND或OR運算子評估篩選。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>變更智慧清單規則邏輯僅適用於篩選器、 **not** 觸發器。

即使上述設定設為ALL，觸發器仍一律評估為OR。  以下是範例：

![](assets/image2014-9-22-14-3a12-3a57.png)

上述智慧清單(簡稱：

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

所以，如果一個人填了表格 **或** 瀏覽頁面時，促銷活動便會根據 **all** 或 **any** 後續篩選器的值，視使用的設定而定。

>[!MORELIKETHIS]
>
>[使用高級智慧清單規則邏輯](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
