---
unique-page-id: 4719316
description: 使用人員帳戶-Marketo文檔——產品文檔
title: 使用人員帳戶
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用人員帳戶{#using-person-accounts}

您可以在Salesforce中設定個人帳戶，以符合您組織的需求。 這是Marketo對待個人賬戶的方式。

>[!NOTE]
>
>預設的Salesforce帳戶是商業帳戶。 您的Salesforce管理員需要個別設定個人帳戶。

## 什麼是個人帳戶？{#what-is-a-person-account}

人員帳戶與Salesforce中的帳戶物件非常相似。 不過，人員帳戶可同時存取帳戶欄位和連絡人欄位。

## 當一個人帳戶與Marketo同步時會發生什麼？{#what-happens-when-a-person-account-is-synced-to-marketo}

人員帳戶與Marketo同步，既是公司，也是個人。

>[!NOTE]
>
>人員帳戶的自訂欄位會複製至Marketo的公司和人員。

## 如何區分商業帳戶和個人帳戶？{#how-do-i-differentiate-business-accounts-and-person-accounts}

使用智慧型清單中的&#x200B;**是人員帳戶**&#x200B;篩選器，將人員帳戶與標準商業帳戶分開。

## 我的個人帳戶資訊顯示在Marketo銷售分析中的位置？{#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

與人員帳戶相關的活動顯示在&#x200B;**Account**&#x200B;面板中。

>[!NOTE]
>
>Marketo銷售分析的&#x200B;**新增至Marketo促銷活動**&#x200B;和&#x200B;**傳送電子郵件**&#x200B;選項目前不適用於個人帳戶。

## 如何將機會關聯至個人帳戶？{#how-do-i-associate-opportunities-to-a-person-account}

Marketo依賴機會聯繫人角色來確定將機會與誰關聯。 您需要為每個人員帳戶添加機會聯繫人角色，以便將機會與Marketo的適當人員聯繫起來。 建議您設定工作流以自動添加業務機會聯繫人角色。

## 我應將哪個電子郵件欄位用於個人帳戶？{#which-email-field-should-i-use-for-person-accounts}

個人帳戶有兩個電子郵件欄位。 使用表單中的&#x200B;**電子郵件地址**&#x200B;欄位（而非&#x200B;**人員電子郵件地址**），以確保Marketo的重複資料消除和其他電子郵件處理正常運作。
