---
unique-page-id: 4719283
description: 瞭解Salesforce同步 — Marketo檔案 — 產品檔案
title: 了解 Salesforce 同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# 瞭解[!DNL Salesforce]同步處理 {#understanding-the-salesforce-sync}

Marketo Engage和Salesforce就像豌豆和胡蘿蔔一樣齊頭並進。 我們保持您的銷售和行銷資料同步。

## 同步如何運作 {#how-sync-works}

Marketo每天都會與[!DNL Salesforce]同步。 每次同步都需要一些時間，然後暫停5分鐘，然後再開始一次。

>[!NOTE]
>
>您的訂閱中第一次同步處理可能需要數小時甚至數天的時間，因為Marketo正在從[!DNL Salesforce]複製整個資料庫。 之後，每個同步通常需要數秒或數分鐘的時間，而且只會同步已變更的資料。

![](assets/sync-illustration.png)

[!DNL Salesforce]與Marketo之間的同步僅針對潛在客戶、聯絡人及[!DNL Salesforce]行銷活動進行雙向同步。 在這些情況下，只要您在[!DNL Salesforce]或Marketo中進行變更，您的更新就會反映在兩個系統中。 所有其他同步僅從[!DNL Salesforce]到Marketo。 按一下下列連結，以取得每個專案的詳細資訊。

## 什麼在Marketo和[!DNL Salesforce]之間同步？ {#what-is-synced-between-marketo-and-salesforce}

* [個銷售機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [連絡人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [個機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce行銷活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [自訂物件](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>您在Marketo中為Salesforce[輸入的](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}認證可用來同步資料。 只有這些認證有權存取的資料才會包括在內。

Marketo與[!DNL Salesforce]的同步處理是世界上最強大的同步處理功能。 感覺就像魔術一樣；變更完成，另一個系統即刻更新。
