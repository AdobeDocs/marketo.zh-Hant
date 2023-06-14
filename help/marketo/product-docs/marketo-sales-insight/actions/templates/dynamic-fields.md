---
description: 動態欄位 — Marketo檔案 — 產品檔案
title: 動態欄位
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: 6d4a093d0ce0158028177cc4a4088526ccf79f9d
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 動態欄位 {#dynamic-fields}

我們可讓您使用預先定義的屬性，將電子郵件範本個人化，例如 `{{first_name}}` 或 `{{company}}`. 這些欄位可讓您傳送電子郵件給多個連絡人，並自動完成這些欄位，而不需為每個連絡人分別輸入這些欄位。

>[!TIP]
>
>「first_name」和「company」欄位是唯一會同時檢視Sales Insight Actions和Salesforce的欄位。 這表示如果連絡人不存在於 [網頁應用程式](https://toutapp.com/login)，我們會檢視Salesforce，看看是否能找到具有相符電子郵件地址的聯絡人/潛在客戶記錄。 然後我們會使用該記錄中的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在 **範本與行銷活動**，找到您要編輯的範本並按一下 **編輯範本**.

1. 按一下 **插入動態欄位**.

   >[!NOTE]
   >
   >以電子郵件傳送存在於銷售分析動作中的聯絡人時，您可以使用基本動態欄位。 這些會直接從連絡人提取。

如果您要傳送電子郵件給Salesforce中的連絡人，您可以利用Salesforce動態欄位。 這些全都以「sfdc」開頭。 只要您連線至Salesforce，這些欄位就會直接呼叫Salesforce中的銷售機會/聯絡人，以填入範本中的資訊。

## 在主旨行中插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只要手動將它們複製並貼到電子郵件的主旨欄位中即可，請注意確保您具有正確的格式。

## 動態欄位預設值 {#dynamic-field-default-values}

將動態欄位新增至電子郵件範本時，您可以新增一個預設值，如果沒有其他可用的值，動態欄位將解析成該值。

若要這麼做，請在動態欄位標籤後新增「|」，然後新增「default：」（兩者不含引號）。 然後，如果找不到其他值，請新增您想要欄位解析為的值（用引號括住）。

**範例：**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 動態欄位字彙表 {#dynamic-fields-glossary}

在Sales Insight Actions中建立範本時，我們一律建議您使用 **插入動態欄位** 按鈕。

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
* 使用時 `{{company_friendly}}`，請務必在聯絡資料中以逗號分隔Inc.或Co.。 這就是Sales Insight Actions在提取值時知道要移除哪些專案的方式。
* 我們可讓您使用預先定義的屬性，將電子郵件範本個人化，例如 `{{my_name}}` 或 `{{my_title}}`. 這些欄位可讓您在電子郵件範本中快速參考自己。

>[!TIP]
>
>如果您的動態欄位未填入，請檢視 [本文](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
