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

## 如何在兩個系統之間保持機會詳細資訊的同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是一種方式：從Salesforce到Marketo。 Salesforce中商機的更新會同步至Marketo。

>[!NOTE]
>
>此 [您在Marketo中輸入的Salesforce憑據](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用於同步資料。 只會包含這些憑證可存取的資料。

## 我可以啟動機會同步嗎？ {#can-i-initiate-an-opportunity-sync}

不行。Salesforce中對任何機會的變更會自動同步至Marketo。

## Marketo是否在Opportunity Amount中支援多種貨幣？ {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不，Marketo只支援一種貨幣。 商機量將與Salesforce同步，但貨幣將為 [預設貨幣](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) 在Marketo訂閱中。

## Marketo如何關聯機會和聯繫人？ {#how-does-marketo-associate-opportunities-and-contacts}

Marketo關聯商機和聯繫人使用 [機會聯繫人角色](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). 未分配任何聯繫人角色的業務機會將同步到Marketo，但不屬於任何人。 例如，此人將不符合Has Opportunity篩選條件。

## 我如何看到一個人的所有機會？ {#how-can-i-see-all-the-opportunities-of-a-person}

您可以在 **機會資訊** 標籤 [人員詳細資訊](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 頁面。

## 哪些觸發器/篩選器與商機有關？ {#what-are-the-triggers-filters-related-to-opportunity}

觸發器：

* 新增至商機
* 從銷售機會中刪除
* 已更新機會

篩選器:

* 有機會
* Opportunity已更新/未更新Opportunity
* 已添加到Opportunity/Not已添加到Opportunity
* 已從Opportunity中刪除/未從Opportunity中刪除
* 總產量
* Opty數
* 預期總營收

>[!TIP]
>
>查看篩選器和觸發器的限制。 裡面有很多很酷的細節。
>
>在Salesforce中，在opportunity對象中建立一個新欄位，它將自動成為一個約束！
