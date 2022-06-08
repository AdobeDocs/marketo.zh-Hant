---
unique-page-id: 2953467
description: SFDC同步 — 機會同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 機會同步
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# SFDC同步：機會同步 {#sfdc-sync-opportunity-sync}

## 如何使兩個系統之間的機會詳細資訊保持同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是一種方式：從Salesforce到Marketo。 Salesforce中商機的更新將同步到Marketo。

>[!NOTE]
>
>的 [您在Marketo為Salesforce輸入的憑據](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用於同步資料。 將只包括那些憑據有權訪問的資料。

## 是否可以啟動機會同步？ {#can-i-initiate-an-opportunity-sync}

不行。對Salesforce中任何機會的更改將自動同步到Marketo。

## Marketo是否支援Opportunity Amount中的多種貨幣？ {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不，Marketo只支援一種貨幣。 商機金額將與Salesforce同步，但幣種將是 [預設貨幣](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) 你的Marketo訂閱。

## Marketo如何聯繫機會和聯繫人？ {#how-does-marketo-associate-opportunities-and-contacts}

Marketo聯營商機及聯繫人 [機會聯繫人角色](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)。 未分配任何聯繫人角色的Opportunity將同步到Marketo，但不屬於任何人。 例如，此人將不符合Has Opportunity篩選器。

## 我怎麼能看到一個人的所有機會？ {#how-can-i-see-all-the-opportunities-of-a-person}

您可以在 **機會資訊** 的 [人員詳細資訊](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 的子菜單。

## 哪些觸發器/篩選器與機會相關？ {#what-are-the-triggers-filters-related-to-opportunity}

觸發器：

* 已添加到機會
* 從機會中刪除
* 機會已更新

篩選器:

* 有機會
* 已更新業務機會/未更新業務機會
* 已添加到Opportunity/未添加到Opportunity
* 已從Opportunity中刪除/未從Opportunity中刪除
* 產品總額
* Optys數
* 預期業務收入合計

>[!TIP]
>
>檢出篩選器和觸發器上的約束。 裡面有很多很酷的細節。
>
>只需在Salesforce中的opportunity對象中建立一個新欄位，它就會自動成為一個約束！
