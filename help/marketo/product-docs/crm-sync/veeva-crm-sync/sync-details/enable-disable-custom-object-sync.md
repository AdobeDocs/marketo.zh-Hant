---
description: 啟用/停用自訂物件同步 — Marketo檔案 — 產品檔案
title: 啟用/禁用自定義對象同步
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 啟用/禁用自定義對象同步 {#enable-disable-custom-object-sync}

在Veva CRM例項中建立的自訂物件也可能是Marketo Engage的一部分。 下面是如何設定它。

## 啟用或停用自訂物件同步 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**需要管理員權限**

1. 在Marketo中，按一下 **管理**，然後 **Veva對象同步**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. 如果這是您的第一個自定義對象，請按一下「同步架構」。 否則，按一下 **重新整理結構** 以確保您擁有最新的。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. 如果全域同步正在執行，請按一下 **禁用全局同步**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veva自訂物件結構的同步可能需要幾分鐘的時間。

1. 按一下 **重新整理結構**.

   ![](assets/enable-disable-custom-object-sync-4.png)

選擇要同步的對象，然後按一下啟用同步。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo只有在自訂物件與Veva CRM中的「連絡人」或「帳戶」物件有直接關係時，才能同步該物件。

1. 按一下 **啟用同步** 。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 返回Veeva標籤，然後按一下 **啟用同步**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## 使用自訂物件 {#using-your-custom-objects}

>[!NOTE]
>
>您無法在具有觸發器的智慧型行銷活動中使用自訂物件。

1. 在Smart List中，拖動「Has Opportunity」過濾器，並將設定為 **True**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. （可選）使用篩選約束來縮小焦點。

   ![](assets/enable-disable-custom-object-sync-9.png)

太棒了！ 您現在可以在智慧型行銷活動和智慧清單中使用此自訂物件的資料。

>[!MORELIKETHIS]
>
>[將自定義對象欄位添加/刪除為智慧清單/觸發器約束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}
