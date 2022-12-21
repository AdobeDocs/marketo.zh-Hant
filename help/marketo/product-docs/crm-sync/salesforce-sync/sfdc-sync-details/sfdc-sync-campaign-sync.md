---
unique-page-id: 2953469
description: SFDC同步 — 促銷活動同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 促銷活動同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# SFDC同步：促銷活動同步 {#sfdc-sync-campaign-sync}

Marketo程式可與Salesforce促銷活動同步。 以下是運作方式的概觀。

## 為何應將Marketo計畫與Salesforce行銷活動同步？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo計畫的強大功能。
* 讓成員及其狀態在Marketo計畫和Salesforce促銷活動之間保持同步。
* 點選Marketo和Salesforce中的報表功能。

## 如何同步Marketo計畫和Salesforce促銷活動？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以選擇在方案和Salesforce促銷活動之間建立一對一對應。

![](assets/image2015-7-8-9-3a43-3a8.png)

此 **[頻道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** 和 **[期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** 在Marketo中同步至Salesforce作為 **行銷活動類型** 和 **實際成本**. 此同步為 **單向**，從Marketo到Salesforce。

Marketo **方案成員** 和 **[晉升狀態](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** 與保持同步 **Salesforce促銷活動成員** 和 **活動成員雕像**. 這是 **雙向同步**，因此在Marketo或Salesforce中所做的任何變更都會反映在這兩個系統中。

>[!NOTE]
>
>如果Marketo計畫中有成員不存在於Salesforce中，則Marketo會在Salesforce中將這些人員建立為銷售線索。

## 與促銷活動相關的觸發器/篩選器為何？ {#what-are-the-triggers-filters-related-to-campaigns}

觸發器：

* 新增至SFDC Campaign
* 從SFDC促銷活動中移除
* 在SFDC促銷活動中狀態已變更

篩選器:

* SFDC促銷活動成員

## 我可以將Marketo People添加到我的SFDC促銷活動嗎？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

是，請使用 [添加到SFDC促銷活動流動操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). 如果此人員不存在於Salesforce中，則Marketo會在Salesforce中建立該人員，然後將其新增至促銷活動。

## 我可以使用Marketo從SFDC促銷活動中移除成員嗎？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，請使用 [從SFDC促銷活動流程操作中刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## 我可以使用Marketo變更促銷活動成員狀態嗎？ {#can-i-change-campaign-member-status-using-marketo}

是，請使用 [更改SFDC促銷活動流程操作中的狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## 為什麼我看不到我的任何Salesforce促銷活動？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

您可以檢查下列項目：

1. 請確定 [促銷活動同步已啟用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. 確認您的 [Marketo同步使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 在Salesforce。

>[!NOTE]
>
>如果您的Salesforce促銷活動和對應的Marketo方案的方案狀態不相容，您可能會收到錯誤訊息。 建議您 [在同步前匹配程式狀態](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [將SFDC促銷活動與計畫同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [了解方案會籍](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [啟用/停用促銷活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [將Marketo同步使用者設為行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

