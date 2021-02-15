---
unique-page-id: 14352509
description: 動態欄位辭彙表——行銷檔案——產品檔案
title: 動態欄位辭彙表
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# 動態欄位辭彙表{#dynamic-fields-glossary}

在Sales Connect中建立模板時，我們始終建議使用&#x200B;**MSE Dynamic Fields**&#x200B;按鈕整合動態欄位。

此工具用於`auto-personalize your email`，並且可以通過`pulling information from the People page`節省大量時間。

| 動態欄位 | 電子郵件中顯示的範例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | 基思 |
| `{{friendly_unsubscribe}}` | 如果你不想再聽我的，請告訴我 |
| `{{my_name}}` | 艾倫·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 資深技術撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**請注意**:

* 如果聯繫人的資訊輸入錯誤或在「人員」頁中缺失，則無法正確提取到模板中。
* `{{company}}`和`{{company_friendly}}`之間的區別在於`{{company_friendly}}`將從您聯繫人的公司名稱中刪除任何正式標題，如Inc., LLC等。
* 使用`{{company_friendly}}`時，請務必在聯絡資訊中以逗號分隔Inc.或Co.。 Sales Connect在提取值時就知道要刪除什麼。

>[!TIP]
>
>您可以針對想要自動提取至電子郵件中的任何項目，建立您自己的[自訂動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)
