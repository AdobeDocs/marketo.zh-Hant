---
unique-page-id: 1900585
description: 將可編輯的章節新增至電子郵件範本v1.0 —— 行銷人員檔案——產品檔案
title: 將可編輯的區段新增至電子郵件範本v1.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# 將可編輯的區段新增至電子郵件範本v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果您要在「電子郵件範本編輯器v1.0」中建立範本，則可在其周圍放置特殊的`<div>`，讓任何區段都可編輯。

>[!NOTE]
>
>**範例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

規則：

1. HTML必須始終有效。
1. 必須包含&#x200B;**mktEditable**&#x200B;類。
1. 該ID在該HTML中必須是唯一的。
1. ID中沒有空格。

>[!CAUTION]
>
>mktEditable語句不能嵌套。

如果您想要在電子郵件範本編輯器v2.0中瞭解如何執行此動作，請參閱[電子郵件範本語法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)。
