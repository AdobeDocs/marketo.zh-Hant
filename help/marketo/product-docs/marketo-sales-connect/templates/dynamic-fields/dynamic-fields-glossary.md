---
unique-page-id: 14352509
description: 動態欄位字彙表 — Marketo檔案 — 產品檔案
title: 動態欄位字彙表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# 動態欄位字彙表 {#dynamic-fields-glossary}

在[!DNL Sales Connect]中建立範本時，我們一律建議使用&#x200B;**[!UICONTROL MSE Dynamic Fields]**&#x200B;按鈕整合動態欄位。

此工具用來`auto-personalize your email`，並由`pulling information from the [!UICONTROL People] page`為您節省大量時間。

| 動態欄位 | 電子郵件中所顯示內容的範例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | 如果您不想再收到我們的電子郵件，請按一下這裡 |
| `{{friendly_unsubscribe}}` | 厭倦了所有的電子郵件？ 請在此通知我 |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn，資深技術撰稿人 — Adobe |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | 資深技術撰稿人 |
| `{{work_website}}` | <https://www.adobe.com> |

**注意事項**：

* 如果連絡人的資訊輸入錯誤或從「人物」頁面遺失，將無法正確地提取到您的範本中。
* `{{company}}`與`{{company_friendly}}`的差異在於`{{company_friendly}}`會從連絡人的公司名稱中移除任何正式標題，例如Inc.、LLC.等。
* 使用`{{company_friendly}}`時，請務必在連絡人詳細資料中以逗號分隔Inc.或Co.。 這是Sales Connect提取值時知道要移除哪些專案的方式。
* 系統會自動將使用者的簽名附加到每封傳送的電子郵件中。 如果使用者使用包含`{{my_signature}}`動態欄位的範本，則系統將填入已放置`{{my_signature}}`動態欄位的簽章。 只是為了避免重複而在此新增。 系統處理`{{team_unsubscribe}}`的方式與啟用全域附加取消訂閱設定時相同。

>[!TIP]
>
>您可以針對您想要自動提取至電子郵件中的任何內容，建立您自己的[自訂動態欄位](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)
