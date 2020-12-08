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


# 動態欄位辭彙表 {#dynamic-fields-glossary}

在Sales Connect中建立範本時，我們一律建議使用 **MSE Dynamic Fields按鈕來整合動態欄位** 。

此工具可讓您 `auto-personalize your email` 節省大量時間 `pulling information from the People page`。

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

* 如果某個聯繫人 `information is entered incorrectly` 在「人員」頁面中有或缺失，請將其放入 `will not pull over correctly` 您的模板中。

* 區別 `{{company}}` 在於， `{{company_friendly}}` 您的聯 `{{company_friendly}}``remove any formal title`絡人的公司名稱會顯示Inc., LLC等。
* 使用時， `{{company_friendly}}`請務必在聯絡資訊中以逗號分隔Inc.或Co.。 Sales Connect在提取值時就知道要刪除什麼。

>[!TIP]
>
>您可以針對想要自動 [提取至電子郵件中的任何項目](http://docs.marketo.com/x/fADb) ，建立自訂的動態欄位

