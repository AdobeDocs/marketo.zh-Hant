---
unique-page-id: 2953459
description: SFDC同步 — 帳戶同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 帳戶同步
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# SFDC 同步：帳戶同步 {#sfdc-sync-account-sync}

Marketo也會將您的帳戶資訊與[!DNL Salesforce]同步。 以下是您應瞭解的一些特定事項！

## 資訊會以何種方式同步？ {#which-way-does-the-information-sync}

只有一種方式：從SFDC到Marketo。

## 更新如何運作？ {#how-do-the-updates-work}

如果您更新Marketo中連絡人的「帳戶」欄位，這會變更Marketo中屬於該帳戶的所有連絡人的值。 它不會同步至SFDC。 不過，下次在SFDC中更新該帳戶時，變更將會覆寫Marketo中的所有帳戶資訊。

## 連絡人可以屬於多個帳戶嗎？  {#can-a-contact-belong-to-multiple-accounts}

不可以。 帳戶可以有多個連絡人，連絡人只能有一個帳戶。

## 我可以從Marketo建立帳戶嗎？ {#can-i-create-accounts-from-marketo}

大多不會。 不過，如果您對個人使用[轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}流程步驟，將會建立新的連絡人、新的帳戶和新的機會。

>[!CAUTION]
>
>此流程步驟的使用案例非常有限。 如果您不確定，就不應該使用。

## [!DNL Salesforce]中帳戶欄位的變更是否會導致每個連絡人的變更資料值活動記錄？  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大部份是這樣。 但是，如果某個帳戶擁有超過5,000個連絡人，且該帳戶上的欄位在SFDC中發生變更，則我們會同步處理變更，但不會記錄5,000多個連絡人的活動。
