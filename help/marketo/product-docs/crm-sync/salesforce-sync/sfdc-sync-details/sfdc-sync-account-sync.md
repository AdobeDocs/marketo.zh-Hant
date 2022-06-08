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

Marketo還將您的帳戶資訊與Salesforce同步。 下面是一些你應該知道的具體事情！

## 資訊以哪種方式同步？ {#which-way-does-the-information-sync}

只有一種方式：從SFDC到Marketo。

## 更新如何工作？ {#how-do-the-updates-work}

如果更新Marketo聯繫人的「帳戶」欄位，則它將更改屬於Marketo該帳戶的所有聯繫人的值。 它不同步到SFDC。 但是，下次在SFDC中更新該帳戶時，更改將覆蓋Marketo的所有帳戶資訊。

## 聯繫人是否屬於多個帳戶？  {#can-a-contact-belong-to-multiple-accounts}

否. 一個帳戶可以有多個聯繫人，一個聯繫人只能有一個帳戶。

## 我能從Marketo建立帳戶嗎？ {#can-i-create-accounts-from-marketo}

大多數情況下，不。 但是，如果您使用 [轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 在人員上執行流步驟，它將建立新聯繫人、新帳戶和新機會。

>[!CAUTION]
>
>此流步驟的用例非常有限。 如果你不確定，你可能不該用它。

## Salesforce中帳戶欄位的更改是否導致每個聯繫人的更改資料值活動日誌？  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大多數情況下，是的。 但是，如果一個帳戶在SFDC中有5,000個以上的聯繫人，並且該帳戶上的欄位更改，我們將同步該更改，但不記錄5,000多個聯繫人的活動。
