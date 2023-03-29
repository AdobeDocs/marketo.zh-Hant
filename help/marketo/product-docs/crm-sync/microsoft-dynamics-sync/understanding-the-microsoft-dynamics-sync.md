---
unique-page-id: 10098625
description: 了解Microsoft Dynamics Sync - Marketo檔案 — 產品檔案
title: 了解Microsoft Dynamics同步
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 了解Microsoft Dynamics同步 {#understanding-the-microsoft-dynamics-sync}

Marketo和Microsoft動態。 我們會保持您的銷售和行銷資料同步。

>[!NOTE]
>
>Marketo目前僅支援與Java 7相容的SSL憑證。

>[!CAUTION]
>
>我們目前不支援Marketo Dynamics Sync的沙箱重新整理。 如果您需要重新整理Dynamics CRM沙箱，則需要新的Marketo沙箱。 如需詳細資訊，請連絡Adobe客戶團隊（您的客戶經理）。

## 同步如何運作 {#how-sync-works}

Marketo會每天持續同步資料與Microsoft Dynamics。 這是使用背景同步完成的，分批完成，而非即時完成。

>[!NOTE]
>
>訂閱中的第一次同步需要幾分鐘到幾小時，具體取決於資料庫的大小。 Marketo會從Dynamics複製整個資料庫。 之後，每次同步通常需要數秒或數分鐘，且只會同步已變更的資料。

Marketo和Dynamics之間的同步是雙向的銷售機會和聯繫人。 如果您在Marketo或Dynamics中進行變更，則兩個系統都會反映您的更新。 所有其他欄位（例如帳戶和機會）只會從Dynamics同步至Marketo。

## Marketo和Microsoft Dynamics之間同步的項目為何？ {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [銷售機會](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [聯繫人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帳戶](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 團隊（SystemUsers組）
* [機會](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自訂實體](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

此 [在Marketo for Dynamics中輸入的憑據](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) 用於同步資料。

>[!NOTE]
>
>如果來源例項已與Microsoft Dynamics整合，則不支援例項複製。
