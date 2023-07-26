---
unique-page-id: 4719316
description: 使用個人帳戶 — Marketo檔案 — 產品檔案
title: 使用個人帳戶
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用個人帳戶 {#using-person-accounts}

個人帳戶可在Salesforce中設定以符合您組織的需求。 以下為Marketo處理個人帳戶的方式。

>[!NOTE]
>
>預設Salesforce帳戶為商業帳戶。 您的Salesforce管理員需要個別設定個人帳戶。

## 什麼是個人帳戶？ {#what-is-a-person-account}

個人帳戶與Salesforce中的帳戶物件非常類似。 不過，個人帳戶可同時存取帳戶欄位和聯絡人欄位。

## 個人帳戶同步至Marketo後會發生什麼事？ {#what-happens-when-a-person-account-is-synced-to-marketo}

個人帳戶會以公司和個人的身分同步至Marketo。

>[!NOTE]
>
>個人帳戶的自訂欄位會複製到Marketo中的公司和個人。

## 如何區分商業帳戶和個人帳戶？ {#how-do-i-differentiate-business-accounts-and-person-accounts}

使用 **為個人帳戶** 在您的智慧清單中篩選，以將個人帳戶與標準企業帳戶分開。

## 我的個人帳戶資訊在Marketo Sales Insight中的哪裡顯示？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

與個人帳戶相關的活動會顯示在 **帳戶** 面板。

>[!NOTE]
>
>Marketo Sales Insight的 **新增至Marketo Campaign** 和 **傳送電子郵件** 選專案前不適用於個人帳戶。

## 如何將機會與個人帳戶建立關聯？ {#how-do-i-associate-opportunities-to-a-person-account}

Marketo取決於機會聯絡人角色，以決定與機會建立關聯的人員。 您需要為每個個人帳戶新增機會聯絡人角色，以將機會連結到Marketo中的適當人員。 建議您設定工作流程，以自動新增機會聯絡人角色。

## 個人帳戶應使用哪個電子郵件欄位？ {#which-email-field-should-i-use-for-person-accounts}

個人帳戶有兩個電子郵件欄位。 使用 **電子郵件地址** 欄位(而非 **個人電子郵件地址**)，以確保Marketo的重複資料刪除與其他電子郵件處理可正常運作。
