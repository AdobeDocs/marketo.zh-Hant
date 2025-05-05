---
unique-page-id: 2953467
description: SFDC Sync - Opportunity Sync - Marketo檔案 — 產品檔案
title: SFDC同步 — 機會同步
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# SFDC同步：機會同步 {#sfdc-sync-opportunity-sync}

## 兩個系統之間的機會詳細資料如何保持同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是單向的：從Salesforce同步到Marketo Engage。 Salesforce中商機的更新將同步至Marketo。

>[!NOTE]
>
>您在Marketo for Salesforce[&#128279;](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}中輸入的認證可用來同步資料。 只有這些認證有權存取的資料才會包括在內。

## 我可以起始機會同步處理嗎？ {#can-i-initiate-an-opportunity-sync}

不行。對Salesforce中任何商機的變更將會自動同步至Marketo。

## Marketo是否支援機會金額中有多種貨幣？ {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

否，Marketo僅支援一種貨幣。 此機會金額將從Salesforce進行同步，但貨幣將是您Marketo訂閱中的[預設貨幣](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription){target="_blank"}。

## Marketo如何關聯機會和聯絡人？ {#how-does-marketo-associate-opportunities-and-contacts}

Marketo使用[商機連絡人角色](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}將商機與連絡人建立關聯。 未指派任何「連絡人角色」的機會會同步至Marketo，但不會屬於任何人。 例如，該人員將不符合擁有機會篩選器的資格。

## 我如何知道個人的所有機會？ {#how-can-i-see-all-the-opportunities-of-a-person}

您可以在[個人詳細資料](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}頁面的&#x200B;**機會資訊**&#x200B;索引標籤中檢視機會清單。

## 與機會相關的觸發器/篩選器為何？ {#what-are-the-triggers-filters-related-to-opportunity}

觸發器：

* 新增至商機
* 已從機會中移除
* 機會已更新

篩選器：

* 有機會
* 機會已更新/未更新機會
* 已新增至Opportunity/未新增至Opportunity
* 已從機會中移除/未從機會中移除
* 總商機金額
* 選件數目
* 總商機預期收入

>[!TIP]
>
>請檢視篩選器和觸發器的限制。 裡面有很多很酷的細節。
>
>只要在Salesforce的機會物件中建立一個新欄位，它就會自動變成限制！
