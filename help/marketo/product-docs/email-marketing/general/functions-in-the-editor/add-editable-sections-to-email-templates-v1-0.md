---
unique-page-id: 1900585
description: 在電子郵件範本v1.0中新增可編輯的區段 — Marketo檔案 — 產品檔案
title: 新增可編輯區段至電子郵件範本 v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 15%

---

# 新增可編輯區段至電子郵件範本 v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果您在電子郵件範本編輯器v1.0中建立範本，您可以將特殊的`<div>`放在任何區段周圍，使其可編輯。

>[!NOTE]
>
>**範例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

規則：

1. HTML必須一律有效。
1. 必須包含&#x200B;**mktEditable**&#x200B;的類別。
1. ID在該HTML中必須是唯一的。
1. ID中沒有空格。

>[!CAUTION]
>
>mktEditable陳述式不可巢狀。

如果您想在電子郵件範本編輯器v2.0中瞭解如何執行此動作，請檢視[電子郵件範本語法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)。
