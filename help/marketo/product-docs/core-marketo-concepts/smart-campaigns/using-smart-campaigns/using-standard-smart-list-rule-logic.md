---
unique-page-id: 1147001
description: 使用標準智慧型清單規則邏輯——行銷檔案——產品檔案
title: 使用標準智慧型清單規則邏輯
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---


# 使用標準智慧型清單規則邏輯 {#using-standard-smart-list-rule-logic}

在建立促銷活動智慧清單時，您可能注意到「使用篩選」選項。 此設定可讓您決定是否需要使用AND或OR運算子來評估篩選。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>變更智慧清單規則邏輯只適用於篩選器， **不適用** 觸發器。

即使上述設定設為ALL，觸發器也一律會評估為OR。  以下是一個例子：

![](assets/image2014-9-22-14-3a12-3a57.png)

上述智慧型清單的字詞如下：`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` 因此，如果某人填寫表單或瀏覽頁面 **** ，促銷活動就會根據**所有**或**任何**後續篩選條件來評估該人，視使用的設定而定。

>[!NOTE]
>
>**相關文章**
>
>* [使用高級智慧清單規則邏輯](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



