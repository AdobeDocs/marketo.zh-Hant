---
unique-page-id: 14352509
description: 動態欄位字彙表 — Marketo檔案 — 產品檔案
title: 動態欄位字彙表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 動態欄位字彙表 {#dynamic-fields-glossary}

在Sales Connect中建立範本時，我們一律建議使用 **MSE動態欄位** 按鈕。

此工具用於 `auto-personalize your email` 省下大量時間 `pulling information from the People page`.

| 動態欄位 | 電子郵件中顯示的範例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | 基思 |
| `{{friendly_unsubscribe}}` | 如果你不想再聽我的話，請告訴我 |
| `{{my_name}}` | 艾倫·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高級技術撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**注意事項**:

* 如果聯繫人的資訊輸入不正確或從「人員」頁中缺失，則無法正確將其拉入您的模板。
* 兩者的差異 `{{company}}` 和 `{{company_friendly}}` 是 `{{company_friendly}}` 將從您聯繫人的公司名稱中刪除任何正式標題，如Inc.、 LLC等。
* 使用時 `{{company_friendly}}`，請務必在聯絡資訊中以逗號分隔Inc.或Co. 。 這是Sales Connect在提取值時知道要刪除的內容的方法。

>[!TIP]
>
>您可以建立自己的 [自訂動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) 想要自動提取到電子郵件中的任何資訊
