---
unique-page-id: 10098625
description: 瞭解Microsoft Dynamics Sync —— 行銷檔案——產品檔案
title: 瞭解Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# 瞭解Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo和Microsoft Dynamics攜手合作。 我們讓您的銷售和行銷資料保持同步。

>[!NOTE]
>
>Marketo目前僅支援與Java 7相容的SSL憑證。

## 同步的運作方式 {#how-sync-works}

Market每天都會持續同步資料與Microsoft Dynamics。 它是使用背景同步，分批完成，而不是即時完成。

>[!NOTE]
>
>訂閱中的首次同步需要數分鐘到數小時，視您的資料庫大小而定。 Market會從Dynamics複製整個資料庫。 之後，每次同步通常需要數秒或數分鐘，而且只同步已變更的資料。

Marketo和Dynamics之間的同步對於潛在客戶和聯繫人是雙向的。 如果您在Marketo或Dynamics中進行變更，您的更新將反映在這兩個系統中。 所有其他欄位（例如帳戶和商機）只會以單一方式同步，從Dynamics到Marketo。

## Marketo和Microsoft Dynamics之間有何同步？ {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [銷售線索](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [聯絡人](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帳戶](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [使用者](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 團隊（系統使用者群組）
* [機會](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自訂實體](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>您在 [Marketo中為Dynamics輸入的憑證](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) ，用來同步資料。

Dynamics同步有許多細微差別和功能。 查看「 [Microsoft Dynamics Sync Details」(](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)Microsoft動態同步詳細資訊)部分中的詳細資訊。

>[!CAUTION]
>
>我們目前不支援Marketo Dynamics Sync的沙盒重新整理。 如果您需要重新整理Dynamics CRM沙盒，將需要新的Marketo沙盒。 如需詳細資訊，請連絡您的客戶成功經理。

>[!NOTE]
>
>**相關文章**
>
>* [同步設定](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Microsoft Dynamics Sync詳細資訊](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

