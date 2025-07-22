---
unique-page-id: 10098625
description: 瞭解 [!DNL Microsoft Dynamics] 同步 — Marketo檔案 — 產品檔案
title: 瞭解Microsoft Dynamics同步
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 1%

---

# 瞭解[!DNL Microsoft Dynamics]同步處理 {#understanding-the-microsoft-dynamics-sync}

Marketo和[!DNL Microsoft Dynamics]一起執行。 我們保持您的銷售和行銷資料同步。

>[!NOTE]
>
>Marketo目前僅支援與Java 7相容的SSL憑證。

>[!CAUTION]
>
>我們目前不支援[!DNL Marketo Dynamics]同步處理的沙箱重新整理。 如果您需要重新整理[!DNL Dynamics] CRM沙箱，則需要新的Marketo沙箱。 請聯絡您的客戶成功案例經理，以瞭解更多詳細資訊。

## 同步如何運作 {#how-sync-works}

Marketo一整天都在與[!DNL Microsoft Dynamics]持續同步資料。 這是使用背景同步來批次完成的，而非即時。

>[!NOTE]
>
>您的訂閱中第一次同步需要數分鐘到數小時的時間，視您的資料庫大小而定。 Marketo會從[!DNL Dynamics]複製整個資料庫。 之後，每個同步通常需要數秒或數分鐘的時間，而且只會同步已變更的資料。

對於潛在客戶與連絡人，Marketo與[!DNL Dynamics]之間的同步是雙向的。 如果您在Marketo或[!DNL Dynamics]中進行變更，您的更新將會反映在兩個系統中。 所有其他欄位（例如帳戶和商機）只會以單向方式同步，從[!DNL Dynamics]到Marketo。

## 什麼在Marketo和[!DNL Microsoft Dynamics]之間同步？ {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [銷售機會](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [聯絡人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帳戶](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 團隊（SystemUsers群組）
* [機會](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自訂實體](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

您在Marketo中為[輸入的 [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)認證可用來同步資料。

>[!NOTE]
>
>如果來源執行個體已與[!DNL Microsoft Dynamics]整合，則不支援執行個體復本。
