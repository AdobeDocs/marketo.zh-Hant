---
unique-page-id: 2953469
description: 瞭解如何將Marketo方案與Salesforce行銷活動同步。 將方案對應至促銷活動，並讓成員與狀態在兩個系統之間保持同步。
title: SFDC同步 — Campaign同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/RnUIcPDeA48j-ioSkepxzv0-0Hmh9n5eTcIAsgdHC4s
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 2%

---

# SFDC 同步：行銷活動同步 {#sfdc-sync-campaign-sync}

Marketo方案可以與[!DNL Salesforce]行銷活動同步。 以下是此運作方式的概觀。

## 為什麼要將Marketo方案與[!DNL Salesforce]行銷活動同步？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo計畫的強大功能。
* 在Marketo方案與[!DNL Salesforce]行銷活動之間保持成員及其狀態同步。
* 點選Marketo和[!DNL Salesforce]中的報告功能。

## Marketo方案和[!DNL Salesforce]行銷活動如何同步？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以選擇在方案與[!DNL Salesforce]行銷活動之間建立一對一的對應。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketo中的&#x200B;**[管道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)**&#x200B;和&#x200B;**[期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)**&#x200B;同步至[!DNL Salesforce]，作為&#x200B;**行銷活動型別**&#x200B;和&#x200B;**實際成本**。 此同步是從Marketo到[!DNL Salesforce]的&#x200B;**單向**。

Marketo **方案成員**&#x200B;及其&#x200B;**[進度狀態](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**&#x200B;與&#x200B;**[!DNL Salesforce]行銷活動成員**&#x200B;和&#x200B;**行銷活動成員狀態**&#x200B;保持同步。 這是&#x200B;**雙向同步**，所以在Marketo或[!DNL Salesforce]中所做的任何變更都會反映在這兩個系統中。

>[!NOTE]
>
>如果Marketo程式中有成員不存在於[!DNL Salesforce]中，Marketo會建立這些人員作為[!DNL Salesforce]中的潛在客戶。

## 與行銷活動相關的觸發器/篩選器有哪些？ {#what-are-the-triggers-filters-related-to-campaigns}

觸發器：

* 新增至SFDC Campaign
* 已從SFDC Campaign中移除
* SFDC Campaign中的狀態已變更

篩選器：

* SFDC 行銷活動的成員

## 我可以將Marketo人員新增至SFDC行銷活動嗎？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

是，使用[新增至SFDC行銷活動流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)。 如果此人員不存在於[!DNL Salesforce]中，Marketo將在[!DNL Salesforce]中建立該人員，然後將他新增至行銷活動。

## 我可以使用Marketo從SFDC行銷活動中移除成員嗎？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，使用[從SFDC Campaign移除流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}。

## 我可以使用Marketo變更行銷活動會員狀態嗎？ {#can-i-change-campaign-member-status-using-marketo}

是，使用SFDC行銷活動流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}中的[變更狀態。

## 為什麼我看不到任何[!DNL Salesforce]行銷活動？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

以下是您可以檢查的專案：

1. 確定已啟用[行銷活動同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
1. 確認您的[Marketo同步使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)是[!DNL Salesforce]中的[行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)。

>[!NOTE]
>
>如果您的[!DNL Salesforce]行銷活動和對應的Marketo程式具有不相容的程式狀態，您可能會收到錯誤訊息。 我們建議您[比對sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)之前的程式狀態。

>[!MORELIKETHIS]
>
>* [將SFDC行銷活動與程式同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [了解方案會籍](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [啟用/停用Campaign同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [將Marketo同步處理使用者設為行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
