---
description: 為何我的動態欄位無法填入 — Marketo檔案 — 產品檔案
title: 為什麼我的動態欄位沒有填入
hide: true
hidefromtoc: true
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: f77a076c243c25f3bff98a82751f51c464712795
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 為什麼我的動態欄位沒有填入 {#why-arent-my-dynamic-fields-filling-out}

動態欄位只有在您使用範本時才有效。 您撰寫的個別一次性電子郵件不會填滿這些內容。

## 檢查內容 {#what-to-check}

Sales Insight Actions中有三種類型的動態欄位：基本、自訂和Salesforce。 基本和自訂功能都可從 [網頁應用程式](https://toutapp.com/login). 如果資訊在Web應用程式中不存在，則欄位將為空白。 Salesforce欄位從 [Salesforce.com](https://salesforce.com).

**疑難排解Salesforce欄位**

Salesforce欄位：例如 `{{sfdc_account_name}}`

* 請確定已正確地與Sales Insight Actions連結。 前往 [設定](https://toutapp.com/login) 頁面，按一下 **管理** 在您的CRM旁邊。

**基本和自訂欄位疑難排解**

輸出基本欄位：例如 `{{company}}`

輸出自訂欄位：例如 `{{custom_field_favorite_movie}}`

* 需要為您的連絡人儲存對應欄位，位於 [人員頁面](https://toutapp.com/next#relationships) 供動態欄位參考。 例如，如果您傳送電子郵件給Mary，並使用 `{{company}}` 欄位，但她的聯繫記錄沒有列出公司，我們將無法填寫。

## 為什麼我的電子郵件在未填入所有動態欄位的情況下傳送？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法填入電子郵件中的所有動態欄位，Sales Insight Actions將阻止您的電子郵件傳出。 **不過**，此規則有一些例外。 有些欄位會傳出空白，或如果能找到值，則自動填入值。 下列是無法填入欄位的這些欄位及其反應方式。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>此 `{{first_name}}` 欄位將在Sales Insight Actions和Salesforce中查看，以嘗試提取資訊。 此清單中的所有其他欄位只會在「銷售分析動作」中查看以填入欄位。
