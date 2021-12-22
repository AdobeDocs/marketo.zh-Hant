---
unique-page-id: 2953384
description: 為自訂實體啟用同步功能 — Marketo檔案 — 產品檔案
title: 為自訂實體啟用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: a5bc634bd3b5ec0849617a9fe366a106691ce149
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 為自訂實體啟用同步 {#enable-sync-for-a-custom-entity}

如果您需要Dynamics的自訂實體資料才能在Marketo中使用，以下說明如何啟用其同步：

>[!NOTE]
>
>**需要管理權限**

>[!NOTE]
>
>當您啟用自訂實體的同步時，Marketo會執行初始同步，以匯入自訂物件的所有資料。

1. 前往 **管理** 區段。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 選擇 **Microsoft Dynamics** 按一下 **禁用同步**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >必須暫時禁用全局同步才能啟用或禁用自定義實體。

1. 在「資料庫管理」下，按一下 **Dynamics實體同步** 連結。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 按一下 **同步架構** 連結。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 選取要同步的實體，然後按一下 **啟用同步**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 選取您要同步的欄位，或以 [約束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和/或智慧清單中的觸發器。 完成後，按一下 **啟用同步**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >在同步過程中，您可能會注意到「動態實體同步」項目從導航樹中消失。 這是預期的行為，它將在同步完成後重新出現。

1. 實體現在會有綠色核取記號。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. 別忘了重新啟用全局同步！

   ![](assets/enable-sync-for-a-custom-entity-8.png)

