---
unique-page-id: 14352602
description: 我的動態欄位未填寫 — Marketo檔案 — 產品檔案
title: 我的動態欄位未填入資訊
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 4%

---

# 我的動態欄位未填入資訊 {#my-dynamic-fields-arent-filling-out}

動態欄位只有在您使用範本時才有作用。 您撰寫的個別一次性電子郵件不會填滿這些內容。

## 檢查內容 {#what-to-check}

[!DNL Sales Connect]中有三種型別的動態欄位： Basic、Custom和[!DNL Salesforce]。 基本和自訂兩者看起來都是從[網頁應用程式](https://toutapp.com/login)提取資訊。 如果資訊不存在於網頁應用程式中，欄位將為空白。 [!DNL Salesforce]欄位從[Salesforce.com](https://salesforce.com)提取資訊。

**疑難排解[!DNL Salesforce]欄位**

[!DNL Salesforce]欄位：例如`{{sfdc_account_name}}`

* 請確定已正確連結[!DNL Sales Connect]。 移至[設定](https://toutapp.com/login)頁面，然後按一下您CRM旁的&#x200B;**[!UICONTROL Manage]**。

**基本和自訂欄位疑難排解**

Tout基本欄位：例如`{{company}}`

Tout自訂欄位：例如`{{custom_field_favorite_movie}}`

* 需要在[人員頁面](https://toutapp.com/next#relationships)中為您的連絡人儲存對應的欄位，以便我們的動態欄位參考。 例如，如果您傳送電子郵件給Mary並使用`{{company}}`欄位，但她的連絡人記錄未列出公司，我們便無法填寫。

## 為什麼我的電子郵件傳送時沒有填入所有動態欄位？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我們無法在電子郵件中填入您的所有動態欄位，[!DNL Sales Connect]將停止寄出您的電子郵件。 **不過**，此規則有一些例外。 有些欄位會傳送空白值，如果可以找到，則會自動填入值。 以下列出這些欄位，以及無法填入欄位時的反應。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>`{{first_name}}`欄位會同時檢視[!DNL Sales Connect]和[!DNL Salesforce]以嘗試提取資訊。 此清單中的所有其他欄位僅在[!DNL Sales Connect]中尋找以填入欄位。
