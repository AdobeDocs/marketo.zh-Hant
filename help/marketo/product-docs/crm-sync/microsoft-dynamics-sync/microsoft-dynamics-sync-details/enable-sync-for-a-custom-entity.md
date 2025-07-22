---
unique-page-id: 2953384
description: 為自訂實體啟用同步 — Marketo檔案 — 產品檔案
title: 為自訂實體啟用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 為自訂實體啟用同步 {#enable-sync-for-a-custom-entity}

如果您需要來自[!DNL Dynamics]的自訂實體資料才能在Marketo中使用，以下說明如何為其啟用同步。

>[!PREREQUISITES]
>
>若要使用自訂物件，它必須關聯至Microsoft Dynamics中的[銷售機會](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md){target="_blank"}、[連絡人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md){target="_blank"}或[帳戶](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md){target="_blank"}物件。

>[!NOTE]
>
>* 當您啟用自訂實體的同步時，Marketo會執行初始同步以引入自訂物件的所有資料。
>* 目前不支援&#x200B;_行銷清單和行銷清單成員_。

>[!IMPORTANT]
>
>Marketo同步使用者需要自訂物件的讀取存取權，才能列出該物件並對其執行同步。

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區段。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 選取&#x200B;**[!UICONTROL Microsoft Dynamics]**&#x200B;並按一下&#x200B;**[!UICONTROL Disable Sync]**。

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >您必須暫時停用全域同步才能啟用或停用自訂實體。

1. 在[!UICONTROL Database Management]底下，按一下&#x200B;**[!UICONTROL Dynamics Entities Sync]**&#x200B;連結。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 按一下&#x200B;**[!UICONTROL Sync schema]**&#x200B;連結。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 選取您要同步的實體，然後按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 選取您要在智慧清單中同步或用作[限制](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)和/或觸發器的欄位。 完成時，按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >在同步處理期間，您可能會注意到&quot;[!UICONTROL Dynamic Entities Sync]&quot;專案會從導覽樹狀結構中消失。 這是預期行為，同步完成後將會重新出現。

1. 該實體現在有綠色核取記號。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. 別忘了重新啟用全域同步處理！

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo僅支援連結至標準實體（一或兩個層級）的自訂實體。
   >
   >* 自訂物件樹可能會顯示同一個物件多次，因為它是與其中一個主要物件的直接連線（例如銷售機會、聯絡人或帳戶，或是透過中介物件的間接連線）。 在這種情況下，請選擇最接近主要物件的物件，然後只選擇一個物件。 多次選擇相同的物件可能會阻礙該自訂物件的同步處理。
