---
unique-page-id: 4719283
description: 了解 Salesforce 同步 - Marketo 文件 - 產品文件
title: 了解 Salesforce 同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '212'
ht-degree: 100%

---

# 了解 [!DNL Salesforce] 同步 {#understanding-the-salesforce-sync}

Marketo Engage 和 Salesforce 就像豌豆和胡蘿蔔一樣天生一對、密不可分。我們會保持您的銷售和行銷資料同步處理。

## 同步的運作方式 {#how-sync-works}

Marketo 和 [!DNL Salesforce] 無時無刻都在進行同步。每次同步都需要一些時間，然後暫停 5 分鐘，接著再次開始。

>[!NOTE]
>
>在您的訂閱中進行的首次同步可能需要數小時或甚至好幾天的時間，因為 Marketo 正在從 [!DNL Salesforce] 複製整個資料庫。之後的每次同步則通常花費幾秒鐘或幾分鐘的時間，而且只會同步已變更的資料。

![](assets/sync-illustration.png)

[!DNL Salesforce] 與 Marketo 之間的同步只會針對銷售線索、聯絡人和 [!DNL Salesforce] 行銷活動進行雙向同步。在這些情況下，只要您在 [!DNL Salesforce] 或 Marketo 中進行變更，您的更新都會同步反映在兩個系統中。所有其他同步則僅支援從 [!DNL Salesforce] 同步至 Marketo。按一下下列連結，以取得每個項目的詳細資料。

## Marketo 和 [!DNL Salesforce] 之間會同步哪些項目？ {#what-is-synced-between-marketo-and-salesforce}

* [銷售線索](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [聯絡人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce 行銷活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [自訂物件](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>[您在 Marketo 中為 Salesforce 輸入的認證](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}會用於同步資料。只有這些認證可存取的資料才會包括在內。

Marketo 與 [!DNL Salesforce] 的同步是世界上最強大的同步處理功能。感覺就像變魔術一樣；變更一完成，另一個系統就快速更新了。
