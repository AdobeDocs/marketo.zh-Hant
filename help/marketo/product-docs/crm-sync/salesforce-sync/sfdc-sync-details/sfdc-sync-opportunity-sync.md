---
unique-page-id: 2953467
description: SFDC同步——機會同步——行銷文檔——產品文檔
title: SFDC同步——機會同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# SFDC同步：機會同步{#sfdc-sync-opportunity-sync}

## 如何在兩個系統之間保持機會詳細資訊的同步？{#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是一種方式：從Salesforce到Marketo。 Salesforce中機會的更新將會同步至Marketo。

>[!NOTE]
>
>您在Marketo中為Salesforce](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)輸入的[憑證可用來同步資料。 只有這些認證有權存取的資料才會包含在內。

## 我是否可以啟動Opportunity Sync?{#can-i-initiate-an-opportunity-sync}

不行。Salesforce中任何商機的變更都會自動同步至Marketo。

## Market是否支援Opportunity Amount中的多種貨幣？{#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不行，Marketo僅支援一種貨幣。 業務機會金額將與Salesforce同步，但貨幣將是您Marketo訂閱中的[預設貨幣](https://docs.marketo.com/display/DOCS/Set+Default+Location+Settings+for+a+Subscription#SetDefaultLocationSettingsforaSubscription-SettheDefaultCurrencySettingsforaSubscription)。

## Market如何將機會和聯繫人關聯起來？{#how-does-marketo-associate-opportunities-and-contacts}

Marketo使用[Opportunity Contact Roles](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)將Opportunity和Contact關聯起來。 未分配任何聯繫人角色的業務機會將同步到Marketo，但不屬於任何人。 例如，該人員將不符合Has Opportunity篩選條件。

## 我如何看到一個人的所有機會？{#how-can-i-see-all-the-opportunities-of-a-person}

您可以在[人員詳細資訊](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)頁的&#x200B;**Opportunity Info**&#x200B;頁籤中查看業務機會清單。

## 哪些觸發器／篩選器與業務機會相關？{#what-are-the-triggers-filters-related-to-opportunity}

觸發器：

* 新增至商機
* 從銷售機會中移除
* 機會已更新

篩選條件：

* 有機會
* Opportunity was Updated/Not Opportunity was Updated
* 已添加到Opportunity/Not已添加到Opportunity
* 已從Opportunity中刪除／未從Opportunity中刪除
* 產品總額
* Optys數
* 預計總營收

>[!TIP]
>
>檢查篩選器和觸發器的限制。 裡面有很多酷炫的細節。
>
>只要在Salesforce中在opportunity物件中建立新欄位，它就會自動變成限制！

Marketo擁有全球最佳的Salesforce同步功能！