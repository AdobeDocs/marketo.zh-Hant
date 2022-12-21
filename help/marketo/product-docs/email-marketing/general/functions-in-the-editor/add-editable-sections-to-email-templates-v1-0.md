---
unique-page-id: 1900585
description: 將可編輯的區段新增至電子郵件範本v1.0 - Marketo檔案 — 產品檔案
title: 將可編輯的區段新增至電子郵件範本v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 1%

---

# 將可編輯的區段新增至電子郵件範本v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果您要在電子郵件範本編輯器v1.0中建立範本，您可以放置特殊的 `<div>` 周圍。

>[!NOTE]
>
>**範例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

規則:

1. HTML必須始終有效。
1. 類別 **mktEditable** 必須包含。
1. 該ID在該HTML中必須是唯一的。
1. ID中沒有空格。

>[!CAUTION]
>
>mktEditable陳述式無法巢狀。

如果您想在電子郵件範本編輯器v2.0中了解如何執行此操作，請查看 [電子郵件範本語法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
