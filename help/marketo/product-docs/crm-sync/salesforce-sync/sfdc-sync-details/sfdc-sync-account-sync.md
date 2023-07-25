---
unique-page-id: 2953459
description: SFDC同步 — 帳戶同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 帳戶同步
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# SFDC同步：帳戶同步 {#sfdc-sync-account-sync}

Marketo也會將您的帳戶資訊與Salesforce同步。 以下是一些您應瞭解的特定事項！

## 資訊會以何種方式同步？ {#which-way-does-the-information-sync}

只有一種方式：從SFDC到Marketo。

## 更新如何運作？ {#how-do-the-updates-work}

如果您更新Marketo中某個連絡人的「帳戶」欄位，它會變更Marketo中屬於該帳戶的所有連絡人的值。 它不會同步至SFDC。 不過，下次在SFDC中更新該帳戶時，變更將會覆寫Marketo中的所有帳戶資訊。

## 連絡人可隸屬於多個帳戶嗎？  {#can-a-contact-belong-to-multiple-accounts}

否. 一個帳戶可以有多個連絡人，一個連絡人只能有一個帳戶。

## 我可以從Marketo建立帳戶嗎？ {#can-i-create-accounts-from-marketo}

大多不會。 不過，如果您使用 [轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 流程步驟在個人上，它將建立新的聯絡人、新的帳戶和新的機會。

>[!CAUTION]
>
>此流程步驟的使用案例非常有限。 如果您不確定，則可能不應使用它。

## Salesforce中帳戶欄位的變更是否會導致每個連絡人的變更資料值活動記錄？  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大部份是這樣。 但是，如果帳戶有超過5,000個連絡人，且在SFDC中該帳戶有欄位變更，我們會同步處理變更，但不會記錄5,000多個連絡人的活動。
