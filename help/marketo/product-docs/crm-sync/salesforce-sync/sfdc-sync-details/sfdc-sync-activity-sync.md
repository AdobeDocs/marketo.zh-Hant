---
unique-page-id: 2953473
description: SFDC同步 — Activity Sync - Marketo檔案 — 產品檔案
title: SFDC同步 — 活動同步
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# SFDC同步：活動同步 {#sfdc-sync-activity-sync}

Marketo Engage也會在Salesforce活動資料上同步。 以下是一些問題和答案。

## Marketo同步處理哪些型別的活動資料？ {#what-types-of-activity-data-does-marketo-sync-over}

Marketo會同步處理潛在客戶或連絡人相關的事件和工作。

## 兩個系統之間的活動詳細資料如何保持同步？ {#how-are-activity-details-kept-in-sync-between-the-two-systems}

從Salesforce同步至Marketo是單向的。 但是您可以在Salesforce中使用 [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} flow step or [Customize Activities Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md){target="_blank"} 至Salesforce。

## 我可以使用Marketo建立任務嗎？ {#can-i-create-a-task-using-marketo}

可以，您可以使用 [建立工作流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## 與活動相關的觸發器/篩選器為何？ {#what-are-the-triggers-filters-related-to-activity}

觸發器

* 活動已記錄
* 活動已更新

篩選器

* 活動已記錄/未記錄活動
* 活動已更新/未更新活動

>[!TIP]
>
>不確定「非活動」的措辭嗎？ 「非」是指非使用狀態篩選器。 如需詳細資訊，請參閱此處： [在智慧清單中使用非使用中篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
