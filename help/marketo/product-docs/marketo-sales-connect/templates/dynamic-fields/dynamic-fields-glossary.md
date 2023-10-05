---
unique-page-id: 14352509
description: 動態欄位字彙表 — Marketo檔案 — 產品檔案
title: 動態欄位字彙表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 動態欄位字彙表 {#dynamic-fields-glossary}

在Sales Connect中建立範本時，我們一律建議使用 **mse動態欄位** 按鈕。

此工具用於 `auto-personalize your email` 為您節省大量時間，盡在 `pulling information from the People page`.

| 動態欄位 | 電子郵件中所顯示內容的範例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | 如果您不想再收到我們的電子郵件，請按一下這裡 |
| `{{friendly_unsubscribe}}` | 厭倦了所有的電子郵件？ 請在此通知我 |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn，資深技術撰稿人 — Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 資深技術撰稿人 |
| `{{work_website}}` | https://www.adobe.com |

**注意事項**：

* 如果連絡人的資訊輸入錯誤或從「人物」頁面遺失，將無法正確地提取到您的範本中。
* 兩者之間的差異 `{{company}}` 和 `{{company_friendly}}` 就是 `{{company_friendly}}` 會從連絡人的公司名稱中移除任何正式名稱，例如Inc.、LLC等。
* 使用時 `{{company_friendly}}`，請務必在聯絡資料中以逗號分隔Inc.或Co. 。 這是Sales Connect提取值時知道要移除哪些專案的方式。
* 系統會自動將使用者的簽名附加到每封傳送的電子郵件中。 如果使用者搭配 `{{my_signature}}` 動態欄位，則系統會填入簽章，其中 `{{my_signature}}` 已放置動態欄位。 只是為了避免重複而在此新增。 系統將處理 `{{team_unsubscribe}}` 與啟用「全域附加取消訂閱」設定時相同。

>[!TIP]
>
>您可以建立自己的 [自訂動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) 任何您想要自動提取至電子郵件中的內容
