---
unique-page-id: 14352602
description: 我的動態欄位無法填寫——行銷檔案——產品檔案
title: 我的動態欄位無法填滿
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# 我的動態欄位無法填滿 {#my-dynamic-fields-arent-filling-out}

動態欄位只有在您使用範本時才能運作。 您撰寫的個別一次性電子郵件將無法填滿這些內容。

## 檢查內容 {#what-to-check}

Sales Connect中有三種類型的動態欄位：基本、自訂和Salesforce。 「基本」和「自訂」都會從Web應用程式 [擷取資訊](http://toutapp.com/login)。 如果資訊不存在於Web應用程式中，欄位將會是空白。 Salesforce欄位從 [Salesforce.com提取資訊](http://salesforce.com)。

`**Troubleshooting Salesforce Fields**`

Salesforce欄位：例如， `{{sfdc_account_name}}`

* 請確定它與Sales Connect已正確連接。 前往「設 [定](http://toutapp.com/next#settings) 」頁面，然後按 **一下** CRM旁的「管理」。

**基本和自訂欄位疑難排解**

輸出基本欄位：例如， `{{company}}`

輸出自訂欄位：例如， `{{custom_field_favorite_movie}}`

* 在「 `he corresponding field needs to be saved for your contact` 人員」頁 [面中](http://toutapp.com/next#relationships) ，以供動態欄位參考。 例如，如果您要傳送電子郵件給Mary並使用欄位，但她的聯絡記錄並未列出公司，我們將無法填寫這個欄位。 `{{company}}`

## 為什麼我的電子郵件會在不填入所有動態欄位的情況下傳送？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法在電子郵件中填入您的所有動態欄位，Sales Connect將會阻止您寄出電子郵件。 **但是**，此規則有一些例外。 有些欄位會傳出空白，或自動填入值（如果我們能找到）。 下面列出這些欄位，以及如果無法填入欄位，它們會如何反應。

`{{first_name}}` =空白

`{{last_name}}` =空白

`{{title}}` =空白

`{{company}}` =「您的公司」

`{{friendly_company}}` =「您的公司」

>[!NOTE]
>
>此欄 `{{first_name}}` 位將會在Sales Connect和Salesforce中尋找，以嘗試提取資訊。 此清單中的所有其他欄位僅在Sales Connect中查找以填充該欄位。

