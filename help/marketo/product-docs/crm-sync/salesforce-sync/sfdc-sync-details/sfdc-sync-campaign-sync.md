---
unique-page-id: 2953469
description: SFDC同步 — Campaign同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — Campaign同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# SFDC同步： Campaign同步 {#sfdc-sync-campaign-sync}

Marketo方案可與Salesforce Campaigns同步。 以下是此運作方式的概觀。

## 為何應將Marketo方案與Salesforce行銷活動同步？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo計畫的強大功能。
* 讓成員及其狀態在Marketo方案與Salesforce Campaign之間保持同步。
* 點選Marketo和Salesforce中的報表功能。

## Marketo計畫和Salesforce行銷活動如何同步？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以選擇在方案和Salesforce行銷活動之間建立一對一的對應。

![](assets/image2015-7-8-9-3a43-3a8.png)

此 **[頻道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** 和 **[期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** 在Marketo中同步至Salesforce做為 **行銷活動型別** 和 **實際成本**. 此同步為 **單向**，從Marketo到Salesforce。

Marketo **方案成員** 及其 **[進度狀態](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** 會保持與 **Salesforce行銷活動成員** 和 **行銷活動會員身分**. 這是 **雙向同步**，因此，在Marketo或Salesforce中所做的任何變更都會反映在這兩個系統中。

>[!NOTE]
>
>如果Marketo程式中有未出現在Salesforce中的成員，Marketo會將這些人員建立為Salesforce中的潛在客戶。

## 與行銷活動相關的觸發器/篩選器有哪些？ {#what-are-the-triggers-filters-related-to-campaigns}

觸發器：

* 已新增至SFDC Campaign
* 已從SFDC Campaign移除
* SFDC Campaign中的狀態已變更

篩選器:

* SFDC Campaign的成員

## 我可以將Marketo人員新增至SFDC行銷活動嗎？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

是，請使用 [新增至SFDC行銷活動流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). 如果此人員不存在於Salesforce中，Marketo將在Salesforce中建立該人員，然後將他新增至促銷活動。

## 我可以使用Marketo從SFDC行銷活動中移除成員嗎？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，請使用 [從SFDC Campaign流程動作中移除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## 我可以使用Marketo變更行銷活動會員狀態嗎？ {#can-i-change-campaign-member-status-using-marketo}

是，請使用 [變更SFDC行銷活動流程動作中的狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## 為什麼我看不到任何Salesforce行銷活動？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

以下是您可以檢查的事項：

1. 確定 [campaign同步已啟用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. 確認您的 [Marketo同步使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) Salesforce中的。

>[!NOTE]
>
>如果您的Salesforce行銷活動和對應的Marketo程式具有不相容的程式狀態，您可能會收到錯誤訊息。 我們建議您 [符合約步前的程式狀態](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [將SFDC行銷活動與程式同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [瞭解計畫成員資格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [啟用/停用Campaign同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [將Marketo同步使用者設為行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)
