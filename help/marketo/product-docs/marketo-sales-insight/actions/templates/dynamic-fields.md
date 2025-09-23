---
description: 動態欄位 — Marketo檔案 — 產品檔案
title: 動態欄位
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 2%

---

# 動態欄位 {#dynamic-fields}

我們允許您使用`{{first_name}}`或`{{company}}`等預先定義的屬性，個人化您的電子郵件範本。 這些欄位可讓您以電子郵件傳送多個連絡人，並自動完成這些欄位，而不需為每個連絡人分別輸入這些欄位。

>[!TIP]
>
>「first_name」和「company」欄位是唯一會同時尋找[!DNL Sales Insight Actions]和[!DNL Salesforce]的欄位。 也就是說，如果連絡人不存在於[網頁應用程式](https://toutapp.com/login)中，我們會檢視[!DNL Salesforce]，看看是否可找到具有相符電子郵件地址的連絡人/潛在客戶記錄。 然後使用該記錄中的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在&#x200B;**[!UICONTROL Templates & Campaigns]**&#x200B;中，找到您要編輯的範本，然後按一下&#x200B;**[!UICONTROL Edit Template]**。

1. 按一下「**[!UICONTROL Insert Dynamic Field]**」。

   >[!NOTE]
   >
   >以電子郵件傳送存在於[!DNL Sales Insight Actions]中的連絡人時，您可以使用基本動態欄位。 這些會直接從連絡人提取。

如果您要傳送電子郵件給存在於[!DNL Salesforce]中的連絡人，您可以利用[!DNL Salesforce]動態欄位。 這些全都以「sfdc」開頭。 只要您連線至[!DNL Salesforce]，這些欄位就會直接呼叫[!DNL Salesforce]中的潛在客戶/連絡人，以填入範本中的資訊。

## 在主旨列插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只要手動複製並貼到電子郵件的主旨欄位中，請務必確保具有正確的格式。

## 動態欄位預設值 {#dynamic-field-default-values}

將動態欄位新增至電子郵件範本時，您可以新增預設值，如果沒有其他可用值，動態欄位將解析該預設值。

若要這麼做，請在動態欄位標籤後新增「|」，然後新增「default：」（兩者不含引號）。 然後，如果找不到其他值，請新增您想要欄位解析到的值（用引號括住）。

**範例：**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 動態欄位字彙表 {#dynamic-fields-glossary}

在[!DNL Sales Insight Actions]中建立範本時，我們一律建議使用&#x200B;**[!UICONTROL Insert Dynamic Field]**&#x200B;按鈕整合動態欄位。

此工具用來`auto-personalize your email`，並由`pulling information from the People page`為您節省大量時間。

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
* 使用`{{company_friendly}}`時，請務必在連絡人詳細資料中以逗號分隔Inc.或Co.。 這就是[!DNL Sales Insight Actions]在提取值時知道要移除哪些專案的方式。
* 我們允許您使用`{{my_name}}`或`{{my_title}}`等預先定義的屬性，個人化您的電子郵件範本。 這些欄位可讓您在電子郵件範本中快速參考自己。
* 系統會自動將使用者的簽名附加到每封傳送的電子郵件中。 如果使用者使用包含`{{my_signature}}`動態欄位的範本，則系統將填入已放置`{{my_signature}}`動態欄位的簽章。 只是為了避免重複而在此新增。 系統處理`{{team_unsubscribe}}`的方式與啟用全域附加取消訂閱設定時相同。

>[!TIP]
>
>如果動態欄位未填入，請檢視[此文章](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md)。
