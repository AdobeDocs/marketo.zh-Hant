---
unique-page-id: 4719283
description: 瞭解Salesforce同步如何讓Marketo和Salesforce資料保持同步。 瞭解已同步的內容，以及雙向同步如何用於潛在客戶和聯絡人。
title: 了解 Salesforce 同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/1H8ol0eKIzfQoQR-Je4jCdZX7R-rWWD63qrhkrsWtyg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 224
ht-degree: 81%

---

# 了解 [!DNL Salesforce] 同步 {#understanding-the-salesforce-sync}

瞭解Salesforce同步如何讓Marketo和Salesforce資料保持同步。

## 同步的運作方式 {#how-sync-works}

Marketo 和 [!DNL Salesforce] 無時無刻都在進行同步。 每次同步都需要一些時間，然後暫停 5 分鐘，接著再次開始。

>[!NOTE]
>
>在您的訂閱中進行的首次同步可能需要數小時或甚至好幾天的時間，因為 Marketo 正在從 [!DNL Salesforce] 複製整個資料庫。 之後的每次同步則通常花費幾秒鐘或幾分鐘的時間，而且只會同步已變更的資料。

![](assets/sync-illustration.png)

[!DNL Salesforce] 與 Marketo 之間的同步只會針對銷售線索、聯絡人和 [!DNL Salesforce] 行銷活動進行雙向同步。 在這些情況下，只要您在 [!DNL Salesforce] 或 Marketo 中進行變更，您的更新都會同步反映在兩個系統中。 所有其他同步則僅支援從 [!DNL Salesforce] 同步至 Marketo。 按一下下列連結，以取得每個項目的詳細資料。

## Marketo 和 [!DNL Salesforce] 之間會同步哪些項目？ {#what-is-synced-between-marketo-and-salesforce}

* [銷售機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [聯絡人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce行銷活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [自訂物件](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [活動](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>[您在 Marketo 中為 Salesforce 輸入的認證](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}會用於同步資料。 只有這些認證可存取的資料才會包括在內。

Marketo 與 [!DNL Salesforce] 的同步是世界上最強大的同步處理功能。 感覺就像變魔術一樣；變更一完成，另一個系統就快速更新了。
