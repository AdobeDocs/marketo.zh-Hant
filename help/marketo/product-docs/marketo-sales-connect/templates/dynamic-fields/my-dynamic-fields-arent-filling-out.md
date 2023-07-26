---
unique-page-id: 14352602
description: 我的動態欄位未填寫 — Marketo檔案 — 產品檔案
title: 我的動態欄位未填寫
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# 我的動態欄位未填寫 {#my-dynamic-fields-arent-filling-out}

動態欄位只有在您使用範本時才有作用。 您撰寫的個別一次性電子郵件不會填滿這些內容。

## 檢查內容 {#what-to-check}

Sales Connect中有三種型別的動態欄位：「基本」、「自訂」和「Salesforce」。 基本和自訂兩者看起來都會從提取資訊 [網頁應用程式](https://toutapp.com/login). 如果資訊不存在於網頁應用程式中，欄位將為空白。 Salesforce欄位提取資訊來源 [Salesforce.com](https://salesforce.com).

**疑難排解Salesforce欄位**

Salesforce欄位：例如 `{{sfdc_account_name}}`

* 請確定已正確連結Sales Connect。 前往 [設定](https://toutapp.com/login) 頁面並按一下 **管理** ，位於您的CRM旁。

**疑難排解基本和自訂欄位**

Tout基本欄位： `{{company}}`

宣傳自訂欄位：例如 `{{custom_field_favorite_movie}}`

* 您的聯絡人需要儲存的對應欄位在 [人員頁面](https://toutapp.com/next#relationships) 以供我們的動態欄位參考。 例如，如果您傳送電子郵件給Mary並使用 `{{company}}` 欄位，但她的連絡人記錄並未列出公司，我們無法填寫。

## 為什麼我的電子郵件傳送時沒有填入所有動態欄位？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法在電子郵件中填入您的所有動態欄位，Sales Connect將停止傳送您的電子郵件。 **但是**，此規則有一些例外。 有些欄位會傳送空白值，如果可以找到，則會自動填入值。 以下列出這些欄位，以及無法填入欄位時的反應。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>此 `{{first_name}}` 欄位會同時檢視Sales Connect和Salesforce以嘗試提取資訊。 此清單中的所有其他欄位只會在Sales Connect中尋找以填入欄位。
