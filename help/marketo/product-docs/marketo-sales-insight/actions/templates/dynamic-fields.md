---
description: 動態欄位 — Marketo檔案 — 產品檔案
title: 動態欄位
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 動態欄位 {#dynamic-fields}

我們可讓您使用預先定義的屬性(例如 `{{first_name}}` 或 `{{company}}`. 這些欄位可讓您傳送電子郵件給多個聯絡人，並自動完成這些欄位，而不必為每個聯絡人個別輸入。

>[!TIP]
>
>「first_name」和「company」欄位是唯一可同時查看Sales Insight Actions和Salesforce的欄位。 這表示如果連絡人不存在於 [網頁應用程式](https://toutapp.com/login)，我們會在Salesforce中查看是否能找到具有相符電子郵件地址的聯絡/銷售機會記錄。 然後，我們會使用該記錄的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在 **範本與行銷活動**，找到您要編輯的範本並按一下 **編輯範本**.

1. 按一下 **插入動態欄位**.

   >[!NOTE]
   >
   >用電子郵件傳送Sales Insight Actions中存在的聯繫人時，您可以使用基本的動態欄位。 這些會直接從聯絡人處拉出。

如果您正在向Salesforce中存在的聯繫人發送電子郵件，則可以利用Salesforce動態欄位。 這些都以「sfdc」開頭。 只要您與Salesforce有連線，這些欄位就會直接呼叫Salesforce中的銷售機會/連絡人，以填入範本中的資訊。

## 在主旨行中插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只需手動複製並貼到電子郵件的主旨欄位，並請務必注意，以確保格式正確。

## 動態欄位字彙表 {#dynamic-fields-glossary}

在Sales Insight Actions中建立範本時，我們一律建議使用 **插入動態欄位** 按鈕。

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
* 使用時 `{{company_friendly}}`，請務必在聯絡資訊中以逗號分隔Inc.或Co. 。 這是Sales Insight Actions提取值時如何移除的內容。
* 我們可讓您使用預先定義的屬性(例如 `{{my_name}}` 或 `{{my_title}}`. 這些欄位可讓您在電子郵件範本中快速參考自己。

>[!TIP]
>
>如果動態欄位未填入，請查看 [這篇文章](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
