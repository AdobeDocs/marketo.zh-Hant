---
unique-page-id: 2953469
description: SFDC同步 — 市場活動同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 市場活動同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# SFDC同步：市場活動同步 {#sfdc-sync-campaign-sync}

Marketo程式可以與Salesforce市場活動同步。 下面是此操作的概述。

## 我為什麼要將Marketo計畫與Salesforce市場活動同步？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo計畫的強大功能。
* 使成員及其狀態在Marketo程式和Salesforce市場活動之間保持同步。
* 利用Marketo和Salesforce中的報告功能。

## Marketo計畫與Salesforce市場活動如何同步？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo，您可以選擇在程式和Salesforce市場活動之間建立一對一映射。

![](assets/image2015-7-8-9-3a43-3a8.png)

的 **[通道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** 和 **[期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** 在Marketo同步到Salesforce **市場活動類型** 和 **實際成本**。 此同步為 **單向**&#x200B;從Marketo到Salesforce。

Marketo **程式成員** 和 **[晉升狀態](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** 與 **Salesforce市場活動成員** 和 **活動成員**。 這是 **雙向同步**&#x200B;因此，在Marketo或Salesforce中所做的任何更改都反映在這兩種系統中。

>[!NOTE]
>
>如果Marketo計畫中的成員在Salesforce中不存在，則Marketo會在Salesforce中建立這些成員作為銷售線索。

## 與市場活動相關的觸發器/篩選器是什麼？ {#what-are-the-triggers-filters-related-to-campaigns}

觸發器：

* 添加到SFDC市場活動
* 已從SFDC市場活動中刪除
* SFDC市場活動中的狀態已更改

篩選器:

* SFDC活動成員

## 是否可以將「Marketo人」添加到我的SFDC活動中？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

是，使用 [添加到SFDC市場活動流活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)。 如果此人在Salesforce中不存在，Marketo將在Salesforce中建立此人，然後將他/她添加到市場活動中。

## 是否可以使用Marketo從SFDC活動中刪除成員？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，使用 [從SFDC市場活動流活動中刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)。

## 我能否使用Marketo更改活動成員狀態？ {#can-i-change-campaign-member-status-using-marketo}

是，使用 [更改SFDC市場活動流活動中的狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)。

## 為什麼我看不到我的Salesforce活動？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

以下是您可以檢查的內容：

1. 確保 [市場活動同步已啟用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
1. 確認 [Marketo同步用戶](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [市場營銷用戶](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 在Salesforce中。

>[!NOTE]
>
>如果您的Salesforce市場活動和映射的Marketo程式具有不相容的程式狀態，則可能會收到錯誤消息。 我們建議你 [在同步之前匹配程式狀態](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)。

>[!MORELIKETHIS]
>
>* [將SFDC市場活動與程式同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [瞭解計畫成員資格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [啟用/禁用市場活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [使Marketo同步用戶成為市場營銷用戶](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

