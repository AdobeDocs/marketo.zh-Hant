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

Marketo也會透過Salesforce活動資料同步。 以下是一些問題和答案。

## Marketo會同步到哪些類型的活動資料？ {#what-types-of-activity-data-does-marketo-sync-over}

Marketo會同步與銷售機會或連絡人相關聯的事件和工作。

## 兩個系統之間如何保持活動詳細資訊的同步？ {#how-are-activity-details-kept-in-sync-between-the-two-systems}

同步是從Salesforce到Marketo的一種方式。 但您可以使用 [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流程步驟或 [自訂活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) 到Salesforce。

## 我可以使用Marketo建立任務嗎？ {#can-i-create-a-task-using-marketo}

是，您可以使用 [建立任務流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## 哪些觸發器/篩選器與活動相關？ {#what-are-the-triggers-filters-related-to-activity}

觸發器

* 活動已記錄
* 活動已更新

篩選器

* 活動已記錄/未記錄活動
* 活動已更新/未更新活動

>[!TIP]
>
>不確定「非活動」的用詞？ 「非」是指閒置篩選器。 請前往這裡深入了解： [在智慧清單中使用不活動篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
