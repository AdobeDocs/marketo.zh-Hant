---
unique-page-id: 3571846
description: Microsoft Dynamics Sync —— 自訂實體同步——行銷檔案——產品檔案
title: Microsoft Dynamics Sync —— 自訂實體同步
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics Sync:自訂實體同步 {#microsoft-dynamics-sync-custom-entity-sync}

如果您需要啟用初始自訂實體同步，讓Dynamics中的資料在Marketo中可用，請以下說明如何進行。

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>若要使用自訂物件，它必須與Dynamics中的 [銷售線索](microsoft-dynamics-sync-lead-sync.md)、 [連絡](microsoft-dynamics-sync-contact-sync.md)或 [](microsoft-dynamics-sync-account-sync.md)帳戶物件關聯。

>[!CAUTION]
>
>在開始自訂實體的同步之前，請確定初始同步已完成（將會透過電子郵件通知您）。

1. 前往「管理員」區段。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 按一下 **禁用同步** ，暫時禁用標準全局同步。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. 安裝支援自訂實體同步的Microsoft Dynamics版本（2_0_0_2之後）。 請參 [閱Marketo Plugin Releases for MIcrosoft Dynamics](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)。
1. 為Marketo Sync使用者提供您計畫同步的任何實體的讀取存取權。
1. 在「資料庫管理」下，按一下** Dynamics Entities Sync**連結。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 按一下「 **同步模式** 」連結可以轉換可用自定義實體的清單。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. 清單同步後，選擇要同步的欄位和要用作智慧清單中 [約束](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和／或觸發器的欄位。 完成後，按一下「 **啟用同步**」。

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. 重新啟用全域同步。

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至一或兩層深之標準實體的自訂實體。

   >[!NOTE]
   >
   >實體名稱最多可包含** 33個字元**。

你好！