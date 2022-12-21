---
description: 自訂物件同步 — Marketo檔案 — 產品檔案
title: 自訂物件同步
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 自訂物件同步 {#custom-object-sync}

在Veva CRM例項中建立的自訂物件也可能是Marketo Engage的一部分。 下面是如何設定它。

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>若要使用自訂物件，它必須與Veeva CRM中的連絡人或帳戶物件相關聯。

## 啟用自訂物件 {#enable-custom-object}

1. 在Marketo中，按一下 **管理**，然後 **Veva對象同步**.

   ![](assets/custom-object-sync-1.png)

1. 如果這是您的第一個自訂物件，請按一下 **同步架構**.

   ![](assets/custom-object-sync-2.png)

1. 按一下 **禁用全局同步**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veva自訂物件結構的初始同步可能需要幾分鐘的時間。

1. 將您要同步的自訂物件拖曳至畫布中。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >自訂物件的名稱必須是唯一的。 Marketo不支援兩個名稱相同的不同自訂物件。

1. 按一下 **啟用同步**.

   ![](assets/custom-object-sync-5.png)

1. 按一下 **啟用同步** 。

   ![](assets/custom-object-sync-6.png)

1. 返回 **韋瓦** 標籤。

   ![](assets/custom-object-sync-7.png)

1. 按一下 **啟用同步**.

   ![](assets/custom-object-sync-8.png)

1. 要查看所有Veeva自定義對象，請按一下「管理」(Admin)和「Veeva對象同步」(Veeva Objects Sync)。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至一至兩層之標準實體的自訂實體。

太棒了！ 您現在可以在智慧型促銷活動和智慧清單中使用此自訂物件的資料。

>[!MORELIKETHIS]
>
>* [正在同步呼叫和呼叫密鑰消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [將自定義對象欄位添加/刪除為智慧清單/觸發器約束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}

