---
unique-page-id: 3571846
description: Microsoft Dynamics Sync —— 自訂實體同步-Marketo文檔——產品文檔
title: Microsoft Dynamics Sync —— 自訂實體同步
exl-id: 1e175bd4-509f-4c1f-a41d-456629e4a8fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics Sync:自訂實體同步{#microsoft-dynamics-sync-custom-entity-sync}

如果您需要啟用初始自訂實體同步，讓Dynamics的資料在Marketo可用，請以下說明如何進行。

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>若要使用自訂物件，它必須與Dynamics中的[lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)、[contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)或[account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)物件相關聯。

>[!CAUTION]
>
>在開始自訂實體的同步之前，請確定初始同步已完成（將會透過電子郵件通知您）。

1. 前往「管理員」區段。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 按一下&#x200B;**禁用同步**&#x200B;可暫時禁用標準全局同步。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. 安裝支援自訂實體同步的Microsoft Dynamics版本（2_0_0_2之後）。 請參閱[MarketoPlugin Releases for MIcrosoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)。

1. 為「Marketo同步用戶」授予您計畫同步的任何實體的讀權限。

1. 在「資料庫管理」下，按一下&#x200B;**Dynamics Entities Sync**&#x200B;連結。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 按一下&#x200B;**同步模式**&#x200B;連結可以轉換可用的自定義實體清單。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. 清單同步後，選擇要同步的欄位和要用作智慧清單中[constraints](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)和／或觸發器的欄位。 完成後，按一下「啟用同步」。****

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. 重新啟用全域同步。

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至一或兩層深之標準實體的自訂實體。

   >[!NOTE]
   >
   >實體名稱最多可包含&#x200B;**33個字元**。

你好！
