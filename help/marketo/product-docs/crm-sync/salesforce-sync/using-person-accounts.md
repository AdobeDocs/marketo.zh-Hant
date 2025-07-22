---
unique-page-id: 4719316
description: 使用個人帳戶 — Marketo檔案 — 產品檔案
title: 使用個人帳戶
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# 使用個人帳戶 {#using-person-accounts}

您可以在Salesforce中設定個人帳戶，以符合貴組織的需求。 以下為Marketo Engage處理個人帳戶的方式。

>[!NOTE]
>
>預設[!DNL Salesforce]帳戶為商業帳戶。 您的[!DNL Salesforce]管理員需要個別設定個人帳戶。

## 什麼是個人帳戶？ {#what-is-a-person-account}

個人帳戶與[!DNL Salesforce]中的帳戶物件非常類似。 不過，個人帳戶可同時存取帳戶欄位和聯絡人欄位。

## 個人帳戶同步至Marketo後會發生什麼事？ {#what-happens-when-a-person-account-is-synced-to-marketo}

個人帳戶會以公司和個人的身分同步至Marketo。

>[!NOTE]
>
>個人帳戶的自訂欄位會複製到Marketo中的公司和個人。

## 如何區分商業帳戶和個人帳戶？ {#how-do-i-differentiate-business-accounts-and-person-accounts}

使用智慧清單中的「Is Person Account」篩選器，將個人帳戶與標準商業帳戶分開。

## 我的個人帳戶資訊顯示在Marketo Sales Insight中的何處？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

與個人帳戶相關的活動會顯示在&#x200B;**[!UICONTROL Account]**&#x200B;面板中。

>[!NOTE]
>
>Marketo Sales Insight的&#x200B;**[!UICONTROL Add to Marketo Campaign]**&#x200B;和&#x200B;**[!UICONTROL Send Email]**&#x200B;選專案前不適用於個人帳戶。

## 如何將機會與個人帳戶建立關聯？ {#how-do-i-associate-opportunities-to-a-person-account}

Marketo取決於機會聯絡人角色，以決定與機會建立關聯的人員。 您需要為每個個人帳戶新增機會聯絡人角色，以將機會連結到Marketo中的適當人員。 建議您設定工作流程，以自動新增機會聯絡人角色。

## 個人帳戶應使用哪個電子郵件欄位？ {#which-email-field-should-i-use-for-person-accounts}

個人帳戶有兩個電子郵件欄位。 在您的表單中使用&#x200B;**[!UICONTROL Email Address]**&#x200B;欄位（而非&#x200B;**[!UICONTROL Person Email Address]**）來確保Marketo的重複資料刪除與其他電子郵件處理可正常運作。
