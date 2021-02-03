---
unique-page-id: 2953469
description: SFDC同步——促銷活動同步——行銷人員文檔——產品文檔
title: SFDC同步——促銷活動同步
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# SFDC同步：促銷活動同步{#sfdc-sync-campaign-sync}

Marketo程式可與Salesforce促銷活動同步。 以下是其運作方式的概述。

## 我為何應將Marketo程式與Salesforce促銷活動同步？{#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo程式的強大功能。
* 讓成員及其狀態在Marketo程式和Salesforce促銷活動之間保持同步。
* 運用Marketo和Salesforce中的報告功能。

## Marketo計畫與Salesforce促銷活動之間如何同步？{#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以選擇在方案和Salesforce促銷活動之間建立一對一對應。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketo中的&#x200B;**[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)**&#x200B;和&#x200B;**[期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)**&#x200B;會以&#x200B;**促銷活動類型**&#x200B;和&#x200B;**實際成本**&#x200B;的形式同步至Salesforce。 此同步是從Market到Salesforce的&#x200B;**單向**。

行銷人員&#x200B;**方案成員**&#x200B;及其&#x200B;**[晉升狀態](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**&#x200B;與&#x200B;**Salesforce促銷活動成員**&#x200B;和&#x200B;**促銷活動成員狀態**&#x200B;保持同步。 這是&#x200B;**雙向同步**，因此在Marketo或Salesforce中所做的任何變更都會反映在這兩個系統中。

>[!NOTE]
>
>如果Marketo程式中有成員不存在於Salesforce中，Marketo會在Salesforce中建立這些人作為銷售線索。

## 哪些觸發器／篩選器與促銷活動相關？{#what-are-the-triggers-filters-related-to-campaigns}

觸發器：

* 新增至SFDC促銷活動
* 從SFDC促銷活動中移除
* SFDC促銷活動中的狀態已更改

篩選條件：

* SFDC促銷活動成員

## 我可以將Marketing to People添加到我的SFDC促銷活動中嗎？{#can-i-add-marketo-people-to-my-sfdc-campaign}

是，請使用[添加到SFDC促銷活動流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)。 如果此人員不存在於Salesforce中，Marketo會在Salesforce中建立此人員，然後將其新增至促銷活動。

## 我是否可以使用Marketo從SFDC促銷活動中移除成員？{#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是的，請使用[從SFDC促銷活動流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)。

## 我可以使用Marketo變更促銷活動成員狀態嗎？{#can-i-change-campaign-member-status-using-marketo}

是的，請使用[在SFDC促銷活動流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)中更改狀態。

## 我為什麼看不到任何Salesforce促銷活動？{#why-cant-i-see-any-of-my-salesforce-campaigns}

您可以檢查以下事項：

1. 請確定[促銷活動同步已啟用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
1. 確認您的[Marketo Sync使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)是Salesforce中的[Marketing使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)。

>[!NOTE]
>
>如果您的Salesforce促銷活動和映射的Marketo程式有不相容的程式狀態，您可能會收到錯誤訊息。 我們建議您[在sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)之前匹配程式狀態。

>[!MORELIKETHIS]
>
>* [將SFDC促銷活動與計畫同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [瞭解方案會籍](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [啟用／停用促銷活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [讓Marketo將使用者同步為行銷使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

