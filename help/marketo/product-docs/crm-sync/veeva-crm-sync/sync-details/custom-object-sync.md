---
description: 自訂物件同步 — Marketo檔案 — 產品檔案
title: 自訂物件同步
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# 自訂物件同步 {#custom-object-sync}

在Veeva CRM執行個體中建立的自訂物件也可以是Marketo Engage的一部分。 以下說明設定方法。

>[!NOTE]
>
>**需要管理員許可權**

>[!PREREQUISITES]
>
>若要使用自訂物件，必須將其與Veeva CRM中的連絡人或帳戶物件相關聯。

## 啟用自訂物件 {#enable-custom-object}

1. 在Marketo中，按一下 **管理員**，則 **Veeva物件同步**.

   ![](assets/custom-object-sync-1.png)

1. 如果這是您的第一個自訂物件，請按一下 **同步結構描述**.

   ![](assets/custom-object-sync-2.png)

1. 按一下 **停用全域同步**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva自訂物件結構的初始同步可能需要幾分鐘的時間。

1. 將您要同步的自訂物件拖曳至畫布中。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >自訂物件必須具有唯一的名稱。 Marketo不支援具有相同名稱的兩個不同自訂物件。

1. 按一下 **啟用同步**.

   ![](assets/custom-object-sync-5.png)

1. 按一下 **啟用同步** 再來一次。

   ![](assets/custom-object-sync-6.png)

1. 返回 **Veeva** 標籤。

   ![](assets/custom-object-sync-7.png)

1. 按一下 **啟用同步**.

   ![](assets/custom-object-sync-8.png)

1. 若要檢視所有Veeva自訂物件，請按一下「管理和Veeva物件同步」。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至標準實體的自訂實體，深入一到兩層。

太棒了！ 您現在可以在智慧行銷活動和智慧清單中使用來自此自訂物件的資料。

>[!MORELIKETHIS]
>
>* [正在同步呼叫和呼叫重要訊息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [新增/移除自訂物件欄位作為智慧清單/觸發條件約束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
