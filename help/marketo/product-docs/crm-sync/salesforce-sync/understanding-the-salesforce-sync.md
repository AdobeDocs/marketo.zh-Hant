---
unique-page-id: 4719283
description: 瞭解Salesforce同步 — Marketo檔案 — 產品檔案
title: 瞭解Salesforce同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# 瞭解Salesforce同步 {#understanding-the-salesforce-sync}

Marketo和Salesforce就像豌豆和胡蘿蔔一樣走到一起。 我們保持您的銷售和行銷資料同步。

## 同步如何運作 {#how-sync-works}

Marketo會每天與Salesforce同步。 每次同步都需要一些時間，然後暫停5分鐘，然後再開始一次。

>[!NOTE]
>
>因為Marketo會從Salesforce複製整個資料庫，所以您訂閱中的首次同步作業可能需要數小時甚至數天的時間。 之後，每個同步通常需要數秒或數分鐘的時間，而且只會同步已變更的資料。

![](assets/sync-illustration.png)

Salesforce和Marketo之間的同步只適用於潛在客戶、聯絡人和Salesforce行銷活動，是雙向的。 在這類情況下，只要您在Salesforce或Marketo中進行變更，您的更新就會反映在這兩個系統中。 所有其他同步僅從Salesforce到Marketo。 按一下下列連結，以取得每個專案的詳細資訊。

## 什麼是Marketo與Salesforce之間同步的？ {#what-is-synced-between-marketo-and-salesforce}

* [銷售機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [連絡人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce行銷活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自訂物件](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>此 [您在Marketo中為Salesforce輸入的認證](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用於同步資料。 只有這些認證有權存取的資料才會包括在內。

Marketo與Salesforce的同步處理是世界上同類產品中最強大的。 感覺就像魔術一樣；變更完成，另一個系統即刻更新。
