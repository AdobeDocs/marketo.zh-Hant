---
unique-page-id: 2953384
description: 啟用自定義實體的同步 — Marketo文檔 — 產品文檔
title: 為自定義實體啟用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: dadaf5bd8e887309d0e9ee8fc25fc58d1c4fbe97
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# 為自定義實體啟用同步 {#enable-sync-for-a-custom-entity}

如果您需要Dynamics中的自定義實體資料在Marketo可用，下面是如何啟用同步。

>[!NOTE]
>
>**需要管理權限**

>[!NOTE]
>
>* 當您為自定義實體啟用同步時，Marketo將執行初始同步，以將自定義對象的所有資料都引入。
>* 市場營銷清單和市場營銷清單成員為 **不支援** 此時此刻。


1. 轉到 **管理** 的子菜單。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 選擇 **Microsoft動力** 按一下 **禁用同步**。

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >必須暫時禁用全局同步才能啟用或禁用自定義實體。

1. 在「資料庫管理」下，按一下 **Dynamics實體同步** 的子菜單。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 按一下 **同步架構** 的子菜單。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 選擇要同步的實體，然後按一下 **啟用同步**。

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 選擇要同步或用作的欄位 [約束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和/或智慧清單中的觸發器。 完成後，按一下 **啟用同步**。

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >在同步過程中，您可能會注意到「動態實體同步」項從導航樹中消失。 這是預期的行為，同步完成後將重新出現。

1. 實體現在具有綠色複選標籤。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. 不要忘記重新啟用全局同步！

   ![](assets/enable-sync-for-a-custom-entity-8.png)
