---
unique-page-id: 4719283
description: 了解Salesforce同步 — Marketo檔案 — 產品檔案
title: 了解Salesforce同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# 了解Salesforce同步 {#understanding-the-salesforce-sync}

Marketo和Salesforce就像豌豆和胡蘿蔔一樣。 我們會保持您的銷售和行銷資料同步。

## 同步如何運作 {#how-sync-works}

Marketo每天都會與Salesforce同步。 每次同步都需要一些時間，然後暫停5分鐘，然後再次開始。

>[!NOTE]
>
>訂閱中的第一次同步可能需要數小時甚至數天，因為Marketo正從Salesforce複製整個資料庫。 之後，每次同步通常需要數秒或數分鐘，且只會同步已變更的資料。

![](assets/sync-illustration.png)

Salesforce與Marketo之間的同步只針對銷售機會、連絡人和Salesforce促銷活動是雙向的。 在這些情況下，每當您在Salesforce或Marketo中進行變更時，您的更新都會反映在這兩個系統中。 所有其他同步僅從Salesforce到Marketo。 按一下下方的連結，以取得每個連結的詳細資訊。

## Marketo和Salesforce之間同步的項目為何？ {#what-is-synced-between-marketo-and-salesforce}

* [銷售機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [聯繫人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce行銷活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自訂物件](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>此 [您在Marketo中輸入的Salesforce憑據](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用於同步資料。 只會包含這些憑證可存取的資料。

Marketo與Salesforce的同步是世界上同類公司中最強大的。 感覺就像魔法；已進行變更，其他系統即將更新。
