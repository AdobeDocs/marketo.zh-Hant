---
unique-page-id: 2953473
description: SFDC同步 — 活動同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 活動同步
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# SFDC同步：活動同步 {#sfdc-sync-activity-sync}

Marketo還通過Salesforce活動資料進行同步。 以下是一些問題和答案。

## Marketo同步的活動資料類型是什麼？ {#what-types-of-activity-data-does-marketo-sync-over}

Marketo在與潛在顧客或聯繫人關聯的事件和任務上同步。

## 活動詳細資訊如何在兩個系統之間保持同步？ {#how-are-activity-details-kept-in-sync-between-the-two-systems}

同步是從Salesforce到Marketo的一種方式。 但是，您可以使用 [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流步驟或 [自定義活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) 到Salesforce。

## 我能否使用Marketo建立任務？ {#can-i-create-a-task-using-marketo}

是的，你可以 [建立任務流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)。

## 與活動相關的觸發器/篩選器是什麼？ {#what-are-the-triggers-filters-related-to-activity}

觸發器

* 活動已記錄
* 活動已更新

篩選器

* 已記錄活動/未記錄活動
* 已更新活動/未更新活動

>[!TIP]
>
>不確定「不活動」的措辭？ 「not」指不活動過濾器。 在此處瞭解有關它們的更多資訊： [在智慧清單中使用不活動過濾器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
