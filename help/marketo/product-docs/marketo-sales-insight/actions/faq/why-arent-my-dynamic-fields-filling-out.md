---
description: 為什麼我的動態欄位沒有填寫？ - Marketo檔案 — 產品檔案
title: 為什麼我的動態欄位沒有填寫？
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 為什麼我的動態欄位沒有填寫？ {#why-arent-my-dynamic-fields-filling-out}

動態欄位只有在您使用範本時才有作用。 您撰寫的個別一次性電子郵件不會填滿這些內容。

## 檢查內容 {#what-to-check}

Sales Insight Actions中有三種動態欄位型別： Basic、Custom和Salesforce。 基本和自訂兩者看起來都是從[網頁應用程式](https://toutapp.com/login){target="_blank"}提取資訊。 如果資訊不存在於網頁應用程式中，欄位將為空白。 Salesforce欄位從[Salesforce.com](https://salesforce.com){target="_blank"}提取資訊。

**疑難排解Salesforce欄位**

Salesforce欄位：例如`{{sfdc_account_name}}`

* 請確定它與Sales Insight動作有正確連線。 移至[設定] (https://toutapp.com/login{target="_blank"}頁面，然後按一下您CRM旁的&#x200B;**管理**。

**基本和自訂欄位疑難排解**

Marketo銷售分析動作基本欄位：例如`{{company}}`

Marketo銷售分析動作自訂欄位：例如`{{custom_field_favorite_movie}}`

* 需要為您在[人員頁面](https://toutapp.com/next#relationships){target="_blank"}中的連絡人儲存對應的欄位，以供我們的動態欄位參考。 例如，如果您傳送電子郵件給Mary並使用`{{company}}`欄位，但她的連絡人記錄未列出公司，我們便無法填寫。

## 為什麼我的電子郵件傳送時沒有填入所有動態欄位？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法填入電子郵件中的所有動態欄位，銷售分析動作將會停止傳送您的電子郵件。 **不過**，此規則有一些例外。 有些欄位會傳送空白值，如果可以找到，則會自動填入值。 以下列出這些欄位，以及無法填入欄位時的反應。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>`{{first_name}}`欄位會同時檢視Sales Insight Actions和Salesforce以嘗試提取資訊。 此清單中的所有其他欄位都只會在「銷售分析動作」中尋找以填入欄位。
