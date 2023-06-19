---
description: 為什麼我的動態欄位沒有填寫？ - Marketo檔案 — 產品檔案
title: 為什麼我的動態欄位沒有填寫？
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 為什麼我的動態欄位沒有填寫？ {#why-arent-my-dynamic-fields-filling-out}

動態欄位只有在您使用範本時才能運作。 您撰寫的個別一次性電子郵件不會填滿。

## 檢查內容 {#what-to-check}

Sales Insight Actions中有三種型別的動態欄位： Basic、Custom和Salesforce。 基本和自訂兩者都會從提取資訊 [網頁應用程式](https://toutapp.com/login){target="_blank"}. If the information does not exist in the web application, the fields will be blank. Salesforce fields pull information from [Salesforce.com](https://salesforce.com){target="_blank"}.

**疑難排解Salesforce欄位**

Salesforce欄位：例如 `{{sfdc_account_name}}`

* 請確定已正確連結銷售分析動作。 前往 [設定](https://toutapp.com/login{target="_blank"} 頁面並按一下 **管理** ，位於您的CRM旁。

**基本欄位和自訂欄位疑難排解**

Marketo銷售分析動作基本欄位：例如 `{{company}}`

Marketo銷售分析動作自訂欄位：例如 `{{custom_field_favorite_movie}}`

* 您需要在以下位置為連絡人儲存對應的欄位： [人員頁面](https://toutapp.com/next#relationships){target="_blank"} 供我們的動態欄位參考。 例如，如果您傳送電子郵件給Mary，並使用 `{{company}}` 欄位，但她的聯絡記錄未列出公司，我們無法填寫。

## 為什麼我的電子郵件傳送時未填入所有動態欄位？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法填入電子郵件中的所有動態欄位，「銷售分析動作」將會停止傳送您的電子郵件。 **但是**，此規則有一些例外。 有些欄位會傳送空白值，或自動填入值（如果可以的話）。 以下列出這些欄位，以及如果無法填入欄位時會如何反應。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>此 `{{first_name}}` 欄位會同時檢視Sales Insight Actions和Salesforce，以嘗試提取資訊。 此清單中的所有其他欄位只會在「銷售分析動作」中尋找以填入欄位。
