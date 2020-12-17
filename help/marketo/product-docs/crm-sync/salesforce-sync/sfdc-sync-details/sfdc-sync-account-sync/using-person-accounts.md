---
unique-page-id: 4719316
description: 使用人員帳戶——行銷人員檔案——產品檔案
title: 使用人員帳戶
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# 使用人員帳戶{#using-person-accounts}

您可以在Salesforce中設定個人帳戶，以符合您組織的需求。 以下是Marketo對待個人帳戶的方式。

>[!NOTE]
>
>預設的Salesforce帳戶是商業帳戶。 您的Salesforce管理員需要個別設定個人帳戶。

## 什麼是個人帳戶？{#what-is-a-person-account}

人員帳戶與Salesforce中的帳戶物件非常相似。 不過，人員帳戶可同時存取帳戶欄位和連絡人欄位。

## 當人員帳戶同步至Marketo時，會發生什麼情況？{#what-happens-when-a-person-account-is-synced-to-marketo}

人員帳戶與Marketo同步為公司和個人。

>[!NOTE]
>
>人員帳戶的自訂欄位會複製至Marketo中的公司與人員。

## 如何區分商業帳戶和個人帳戶？{#how-do-i-differentiate-business-accounts-and-person-accounts}

使用智慧型清單中的&#x200B;**是人員帳戶**&#x200B;篩選器，將人員帳戶與標準商業帳戶分開。

## 我的個人帳戶資訊顯示在Marketo Sales Insight的何處？{#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

與人員帳戶相關的活動顯示在&#x200B;**Account**&#x200B;面板中。

>[!NOTE]
>
>Marketo Sales Insight的**新增至Marketo Campaign **和**傳送電子郵件**選項目前不適用於個人帳戶。

## 如何將機會關聯至個人帳戶？{#how-do-i-associate-opportunities-to-a-person-account}

Marketo取決於業務機會聯繫人角色，以確定要將業務機會關聯到的人員。 您需要為每個人員帳戶添加業務機會聯繫人角色，以便將業務機會與Marketo中的適當人員聯繫起來。 建議您設定工作流以自動添加業務機會聯繫人角色。

## 我應將哪個電子郵件欄位用於個人帳戶？{#which-email-field-should-i-use-for-person-accounts}

個人帳戶有兩個電子郵件欄位。 使用表單中的&#x200B;**電子郵件地址**&#x200B;欄位（而非&#x200B;**人員電子郵件地址**），以確保Marketo的重複資料消除和其他電子郵件處理正常運作。
