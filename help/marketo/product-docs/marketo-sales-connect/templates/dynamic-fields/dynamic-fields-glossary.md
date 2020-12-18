---
unique-page-id: 14352509
description: 動態欄位辭彙表——行銷檔案——產品檔案
title: 動態欄位辭彙表
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[受電子郵件保護]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | 資深技術撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**請注意**:

* 如果聯繫人的`information is entered incorrectly`或在「人員」頁中缺失，則該聯繫人`will not pull over correctly`將放入模板中。

* `{{company}}`和`{{company_friendly}}`之間的區別是，`{{company_friendly}}`會從您聯絡人的公司名稱中`remove any formal title`，例如Inc., LLC.等。
* 使用`{{company_friendly}}`時，請務必在聯絡資訊中以逗號分隔Inc.或Co.。 Sales Connect在提取值時就知道要刪除什麼。

>[!TIP]
>
>您可以針對想要自動提取至電子郵件中的任何項目，建立您自己的[自訂動態欄位](http://docs.marketo.com/x/fADb)

