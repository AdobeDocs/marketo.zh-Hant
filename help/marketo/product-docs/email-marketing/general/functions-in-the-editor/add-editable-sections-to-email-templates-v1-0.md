---
unique-page-id: 1900585
description: 在電子郵件範本v1.0中新增可編輯的區段 — Marketo檔案 — 產品檔案
title: 將可編輯的區段新增至電子郵件範本v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 1%

---

# 將可編輯的區段新增至電子郵件範本v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果您在電子郵件範本編輯器v1.0中建立範本，您可以放置特殊符號讓任何區段可編輯 `<div>` 圍著它。

>[!NOTE]
>
>**範例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

規則:

1. HTML必須一律有效。
1. 的類別 **mktEditable** 必須包含。
1. 該ID在該HTML中必須是唯一的。
1. ID中沒有空格。

>[!CAUTION]
>
>mktEditable陳述式不可巢狀。

如果您想在電子郵件範本編輯器v2.0中瞭解如何執行此操作，請檢視 [電子郵件範本語法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
