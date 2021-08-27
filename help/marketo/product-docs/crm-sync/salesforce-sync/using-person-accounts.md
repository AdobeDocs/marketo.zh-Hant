---
unique-page-id: 4719316
description: 使用人員帳戶 — Marketo檔案 — 產品檔案
title: 使用人員帳戶
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用人員帳戶 {#using-person-accounts}

您可以在Salesforce中設定人員帳戶，以符合您組織的需求。 這是Marketo對待人員帳戶的方式。

>[!NOTE]
>
>預設的Salesforce帳戶是業務帳戶。 您的Salesforce管理員需要個別設定人員帳戶。

## 什麼是人員帳戶？ {#what-is-a-person-account}

人員帳戶與Salesforce中的帳戶物件非常類似。 但是，人員帳戶可以同時訪問帳戶欄位和聯繫人欄位。

## 將人員帳戶同步至Marketo時會發生什麼事？ {#what-happens-when-a-person-account-is-synced-to-marketo}

人員帳戶會以公司和人員身分同步至Marketo。

>[!NOTE]
>
>人員帳戶的自訂欄位會複製到Marketo中的公司和人員。

## 如何區分業務帳戶和人員帳戶？ {#how-do-i-differentiate-business-accounts-and-person-accounts}

在智慧清單中使用&#x200B;**是人員帳戶**&#x200B;篩選器，將人員帳戶與標準業務帳戶分開。

## 我的人員帳戶資訊在Marketo Sales Insight中顯示於何處？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

與人員帳戶相關的活動顯示在&#x200B;**Account**&#x200B;面板中。

>[!NOTE]
>
>Marketo Sales Insight的&#x200B;**新增至Marketo促銷活動**&#x200B;和&#x200B;**傳送電子郵件**&#x200B;選項目前不適用於人員帳戶。

## 如何將機會與人員帳戶關聯？ {#how-do-i-associate-opportunities-to-a-person-account}

Marketo取決於機會聯繫人角色，以確定要將該機會關聯到哪個人員。 您需要為每個人員帳戶添加機會聯繫人角色，以將該機會與Marketo中的適當人員連接。 建議您設定一個工作流以自動添加機會聯繫人角色。

## 我應將哪個電子郵件欄位用於人員帳戶？ {#which-email-field-should-i-use-for-person-accounts}

人員帳戶有兩個電子郵件欄位。 使用表單中的&#x200B;**電子郵件地址**&#x200B;欄位（非&#x200B;**人員電子郵件地址**），確保Marketo的重複資料消除和其他電子郵件處理正常運作。
