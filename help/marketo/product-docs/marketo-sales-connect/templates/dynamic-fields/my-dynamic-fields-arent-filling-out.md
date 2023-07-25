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

動態欄位只有在您使用範本時才能運作。 您撰寫的個別一次性電子郵件不會填滿。

## 檢查內容 {#what-to-check}

Sales Connect中有三種型別的動態欄位： Basic、Custom和Salesforce。 基本和自訂兩者都會從提取資訊 [網頁應用程式](https://toutapp.com/login). 如果資訊不存在於Web應用程式中，欄位將為空白。 Salesforce欄位提取資訊來源 [Salesforce.com](https://salesforce.com).

**疑難排解Salesforce欄位**

Salesforce欄位：例如 `{{sfdc_account_name}}`

* 確定已正確連結Sales Connect。 前往 [設定](https://toutapp.com/login) 頁面並按一下 **管理** ，位於您的CRM旁。

**基本欄位和自訂欄位疑難排解**

Tout基本欄位： `{{company}}`

吹噓自訂欄位：例如 `{{custom_field_favorite_movie}}`

* 您需要在以下位置為連絡人儲存對應的欄位： [人員頁面](https://toutapp.com/next#relationships) 供我們的動態欄位參考。 例如，如果您傳送電子郵件給Mary，並使用 `{{company}}` 欄位，但她的聯絡記錄未列出公司，我們無法填寫。

## 為什麼我的電子郵件傳送時未填入所有動態欄位？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法填入電子郵件中的所有動態欄位，Sales Connect將停止寄出您的電子郵件。 **但是**，此規則有一些例外。 有些欄位會傳送空白值，或自動填入值（如果可以的話）。 以下列出這些欄位，以及如果無法填入欄位時會如何反應。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>此 `{{first_name}}` 欄位會同時檢視Sales Connect和Salesforce以嘗試提取資訊。 此清單中的所有其他欄位只會在Sales Connect中尋找以填入欄位。
