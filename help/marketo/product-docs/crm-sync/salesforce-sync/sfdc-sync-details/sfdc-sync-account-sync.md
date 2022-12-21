---
unique-page-id: 2953459
description: SFDC同步 — 帳戶同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 帳戶同步
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# SFDC同步：帳戶同步 {#sfdc-sync-account-sync}

Marketo也會將您的帳戶資訊與Salesforce同步。 以下是一些您應了解的具體事項！

## 資訊會以哪種方式同步？ {#which-way-does-the-information-sync}

只有一種方式：從SFDC到Marketo。

## 更新如何運作？ {#how-do-the-updates-work}

如果您更新Marketo中某個聯絡人的「帳戶」欄位，它會變更Marketo中屬於該帳戶的所有聯絡人的值。 它不同步到SFDC。 不過，下次在SFDC中更新該帳戶時，變更將會覆寫Marketo中的所有帳戶資訊。

## 聯繫人是否可以屬於多個帳戶？  {#can-a-contact-belong-to-multiple-accounts}

否. 帳戶可以有多個聯繫人，聯繫人只能有一個帳戶。

## 我可以從Marketo建立帳戶嗎？ {#can-i-create-accounts-from-marketo}

大多數情況下，不。 不過，如果您使用 [轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 在人員上執行流動步驟，將建立新的聯繫人、新的帳戶和新的機會。

>[!CAUTION]
>
>此流程步驟的使用案例非常有限。 如果你不確定，你可能不該用。

## Salesforce中的帳戶欄位的變更是否會導致每個聯絡人的「變更資料值活動記錄」？  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大多數情況下，是的。 但是，如果一個帳戶有5,000多個聯繫人，並且SFDC中該帳戶的欄位更改，我們將同步更改，但不會記錄5,000多個聯繫人的活動。
