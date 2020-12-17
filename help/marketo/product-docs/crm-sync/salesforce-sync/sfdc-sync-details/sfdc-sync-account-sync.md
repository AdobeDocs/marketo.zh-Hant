---
unique-page-id: 2953459
description: SFDC同步——帳戶同步——行銷文檔——產品文檔
title: SFDC同步——帳戶同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# SFDC同步：帳戶同步{#sfdc-sync-account-sync}

Market也會將您的帳戶資訊與Salesforce同步。 以下是一些您應該知道的具體內容！

## 資訊會以哪種方式同步？{#which-way-does-the-information-sync}

只有一種方式：從SFDC到行銷人員。

## 這些更新如何運作？{#how-do-the-updates-work}

如果您更新Marketo中某個連絡人的「帳戶」欄位，則會變更Marketo中屬於該帳戶的所有連絡人的值。 它不同步到SFDC。 不過，下次在SFDC中更新該帳戶時，這些變更將覆蓋Marketo中的所有帳戶資訊。

## 連絡人是否屬於多個帳戶？ {#can-a-contact-belong-to-multiple-accounts}

不。 帳戶可以有多個連絡人，而連絡人只能有一個帳戶。

## 我可以從Marketo建立帳戶嗎？{#can-i-create-accounts-from-marketo}

大多數情況下，不。 但是，如果您在人員上使用[轉換人員](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)流程步驟，則將建立新的聯繫人、新的帳戶和新的Opportunity。

>[!CAUTION]
>
>此流程步驟的使用案例非常有限。 如果你不確定，你可能不該用它。

## Salesforce中帳戶欄位的變更是否會導致每個連絡人的「變更資料值」活動記錄？ {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大多數情況下，是的。 但是，如果一個帳戶有5,000個以上的聯繫人，而SFDC中該帳戶上的欄位有更改，我們將同步更改，但不記錄5,000個以上聯繫人的活動。
