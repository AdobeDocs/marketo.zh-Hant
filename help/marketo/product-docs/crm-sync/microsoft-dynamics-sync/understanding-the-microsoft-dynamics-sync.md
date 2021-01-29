---
unique-page-id: 10098625
description: 瞭解Microsoft Dynamics Sync —— 行銷檔案——產品檔案
title: 瞭解Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---


# 瞭解Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo和Microsoft Dynamics攜手合作。 我們讓您的銷售和行銷資料保持同步。

>[!NOTE]
>
>Marketo目前僅支援與Java 7相容的SSL憑證。

## 同步如何運作{#how-sync-works}

Market每天都會持續同步資料與Microsoft Dynamics。 它是使用背景同步，分批完成，而不是即時完成。

>[!NOTE]
>
>訂閱中的首次同步需要數分鐘到數小時，視您的資料庫大小而定。 Market會從Dynamics複製整個資料庫。 之後，每次同步通常需要數秒或數分鐘，而且只同步已變更的資料。

Marketo和Dynamics之間的同步對於潛在客戶和聯繫人是雙向的。 如果您在Marketo或Dynamics中進行變更，您的更新將反映在這兩個系統中。 所有其他欄位（例如帳戶和商機）只會以單一方式同步，從Dynamics到Marketo。

## Marketo和Microsoft Dynamics之間有何同步？{#what-is-synced-between-marketo-and-microsoft-dynamics}

* [銷售線索](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [聯絡人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帳戶](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 團隊（系統使用者群組）
* [機會](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自訂實體](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>您在Marketo中為Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)輸入的[憑證會用來同步資料。

>[!CAUTION]
>
>我們目前不支援Marketo Dynamics Sync的沙盒重新整理。 如果您需要重新整理Dynamics CRM沙盒，將需要新的Marketo沙盒。 如需詳細資訊，請連絡您的客戶成功經理。
