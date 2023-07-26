---
description: 啟用/停用自訂物件同步 — Marketo檔案 — 產品檔案
title: 啟用/停用自訂物件同步
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 啟用/停用自訂物件同步 {#enable-disable-custom-object-sync}

在Veeva CRM執行個體中建立的自訂物件也可以是Marketo Engage的一部分。 以下說明設定方法。

## 啟用或停用自訂物件同步 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**需要管理員許可權**

1. 在Marketo中，按一下 **管理員**，然後 **Veeva物件同步**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. 如果這是您的第一個自訂物件，請按一下「同步結構描述」。 如果沒有，請按一下 **重新整理結構描述** 以確保您擁有最新版本。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. 如果您的全域同步正在執行中，請按一下 **停用全域同步**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >同步Veeva自訂物件結構描述可能需要幾分鐘的時間。

1. 按一下 **重新整理結構描述**.

   ![](assets/enable-disable-custom-object-sync-4.png)

選取您要同步的物件，然後按一下「啟用同步」。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo只有在Veeva CRM中與聯絡人或帳戶物件有直接關係時，才能同步處理自訂物件。

1. 按一下 **啟用同步** 再來一次。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 返回Veeva標籤並按一下 **啟用同步**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## 使用您的自訂物件 {#using-your-custom-objects}

>[!NOTE]
>
>您無法在包含觸發器的智慧行銷活動中使用自訂物件。

1. 在智慧清單中，拖曳至「擁有機會」篩選器上，並將設為 **真**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. 或者，使用篩選條件限制來縮小焦點。

   ![](assets/enable-disable-custom-object-sync-9.png)

太好了！ 您現在可以在智慧行銷活動和智慧清單中使用此自訂物件的資料。

>[!MORELIKETHIS]
>
>[新增/移除自訂物件欄位做為智慧清單/觸發條件約束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
