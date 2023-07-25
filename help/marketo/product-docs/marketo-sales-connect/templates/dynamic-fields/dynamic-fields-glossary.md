---
unique-page-id: 14352509
description: 動態欄位字彙表 — Marketo檔案 — 產品檔案
title: 動態欄位字彙表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 動態欄位字彙表 {#dynamic-fields-glossary}

在Sales Connect中建立範本時，我們一律建議使用 **mse動態欄位** 按鈕。

此工具用於 `auto-personalize your email` 節省您大量的時間，盡在 `pulling information from the People page`.

| 動態欄位 | 電子郵件中顯示的內容範例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | 如果您不想再收到我的消息，請在這裡通知我 |
| `{{my_name}}` | 艾倫·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 資深技術撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**注意事項**：

* 如果連絡人的資訊輸入錯誤或從「人物」頁面遺失，則無法將資訊正確提取到您的範本中。
* 兩者之間的差異 `{{company}}` 和 `{{company_friendly}}` 這點 `{{company_friendly}}` 會從連絡人的公司名稱中移除任何正式名稱，例如Inc.、LLC等。
* 使用時 `{{company_friendly}}`，請務必在聯絡資料中以逗號分隔Inc.或Co.。 這就是Sales Connect提取值時知道要移除哪些專案的方式。

>[!TIP]
>
>您可以建立自己的 [自訂動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) 任何您想要自動提取至電子郵件中的內容
