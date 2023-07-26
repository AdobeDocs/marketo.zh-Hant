---
description: 動態欄位 — Marketo檔案 — 產品檔案
title: 動態欄位
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 動態欄位 {#dynamic-fields}

我們允許您使用預先定義的屬性(例如 `{{first_name}}` 或 `{{company}}`. 這些欄位可讓您以電子郵件傳送多個連絡人，並自動完成這些欄位，而不需為每個連絡人分別輸入這些欄位。

>[!TIP]
>
>「first_name」和「company」欄位是唯一會同時檢視Sales Insight Actions和Salesforce的欄位。 這表示如果連絡人不存在於 [網頁應用程式](https://toutapp.com/login)，我們會檢視Salesforce以確認是否能找到具有相符電子郵件地址的聯絡人/潛在客戶記錄。 然後使用該記錄中的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在 **範本與行銷活動**，找到您要編輯的範本並按一下 **編輯範本**.

1. 按一下 **插入動態欄位**.

   >[!NOTE]
   >
   >當傳送電子郵件給存在於銷售分析動作中的聯絡人時，您可以使用基本的動態欄位。 這些會直接從連絡人提取。

如果您要傳送電子郵件給Salesforce中的聯絡人，則可以利用Salesforce動態欄位。 這些全都以「sfdc」開頭。 只要您有Salesforce的連線，這些欄位就會直接呼叫Salesforce中的銷售機會/聯絡人，在範本中填入資訊。

## 在主旨列插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只要手動複製並貼到電子郵件的主旨欄位中，請務必確保具有正確的格式。

## 動態欄位預設值 {#dynamic-field-default-values}

將動態欄位新增至電子郵件範本時，您可以新增預設值，如果沒有其他可用值，動態欄位將解析該預設值。

若要這麼做，請在動態欄位標籤後新增「|」，然後新增「default：」（兩者不含引號）。 然後，如果找不到其他值，請新增您想要欄位解析到的值（用引號括住）。

**範例：**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 動態欄位字彙表 {#dynamic-fields-glossary}

在「銷售分析動作」中建立範本時，我們一律建議您使用 **插入動態欄位** 按鈕。

此工具用於 `auto-personalize your email` 為您節省大量時間，盡在 `pulling information from the People page`.

| 動態欄位 | 電子郵件中所顯示內容的範例 |
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

* 如果連絡人的資訊輸入錯誤或從「人物」頁面遺失，將無法正確地提取到您的範本中。
* 兩者之間的差異 `{{company}}` 和 `{{company_friendly}}` 就是 `{{company_friendly}}` 會從連絡人的公司名稱中移除任何正式名稱，例如Inc.、LLC等。
* 使用時 `{{company_friendly}}`，請務必在聯絡資料中以逗號分隔Inc.或Co. 。 這就是Sales Insight Actions在提取值時知道要移除哪些專案的方式。
* 我們允許您使用預先定義的屬性(例如 `{{my_name}}` 或 `{{my_title}}`. 這些欄位可讓您在電子郵件範本中快速參考自己。

>[!TIP]
>
>如果您的動態欄位未填入，請檢視 [本文](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
