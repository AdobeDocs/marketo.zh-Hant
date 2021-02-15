---
unique-page-id: 14352602
description: 我的動態欄位無法填寫——行銷檔案——產品檔案
title: 我的動態欄位無法填滿
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# 我的動態欄位未填寫{#my-dynamic-fields-arent-filling-out}

動態欄位只有在您使用範本時才能運作。 您撰寫的個別一次性電子郵件將無法填滿這些內容。

## 檢查{#what-to-check}內容

Sales Connect中有三種類型的動態欄位：基本、自訂和Salesforce。 「基本」和「自定義」都會從[Web應用程式](https://toutapp.com/login)中提取資訊。 如果資訊不存在於Web應用程式中，欄位將會是空白。 Salesforce欄位會從[Salesforce.com](https://salesforce.com)提取資訊。

**疑難排解Salesforce欄位**

Salesforce欄位：例如，`{{sfdc_account_name}}`

* 請確定它與Sales Connect已正確連接。 前往[Settings](https://toutapp.com/login)頁面，然後按一下CRM旁的&#x200B;**Manage**。

**基本和自訂欄位疑難排解**

輸出基本欄位：例如，`{{company}}`

輸出自訂欄位：例如，`{{custom_field_favorite_movie}}`

* 您必須在[人員頁面](https://toutapp.com/next#relationships)中儲存對應欄位，才能參考動態欄位。 例如，如果您要傳送電子郵件給Mary並使用`{{company}}`欄位，但她的聯絡記錄未列出公司，我們將無法填寫。

## 為什麼我的電子郵件會在不填入所有動態欄位的情況下傳送？{#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法在電子郵件中填入您的所有動態欄位，Sales Connect將會阻止您寄出電子郵件。 **但是**，此規則有一些例外。有些欄位會傳出空白，或自動填入值（如果我們能找到）。 下面列出這些欄位，以及如果無法填入欄位，它們會如何反應。

`{{first_name}}` =空白

`{{last_name}}` =空白

`{{title}}` =空白

`{{company}}` =「您的公司」

`{{friendly_company}}` =「您的公司」

>[!NOTE]
>
>`{{first_name}}`欄位會在Sales Connect和Salesforce中尋找以嘗試提取資訊。 此清單中的所有其他欄位僅在Sales Connect中查找以填充該欄位。
