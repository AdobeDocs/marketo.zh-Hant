---
unique-page-id: 1147001
description: 使用標準智慧型清單規則邏輯——行銷檔案——產品檔案
title: 使用標準智慧型清單規則邏輯
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# 使用標準智慧清單規則邏輯{#using-standard-smart-list-rule-logic}

在建立促銷活動智慧清單時，您可能注意到「使用篩選」選項。 此設定可讓您決定是否需要使用AND或OR運算子來評估篩選。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>變更智慧型清單規則邏輯僅適用於篩選器，**not**&#x200B;觸發器。

即使上述設定設為ALL，觸發器也一律會評估為OR。  以下是一個例子：

![](assets/image2014-9-22-14-3a12-3a57.png)

上述智慧型清單的字詞如下：
`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>`因此，如果某人填寫了&#x200B;**或**&#x200B;表單，則促銷活動會根據後續篩選的**all **或**any **評估該人，視使用的設定而定。

>[!MORELIKETHIS]
>
>* [使用高級智慧清單規則邏輯](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



