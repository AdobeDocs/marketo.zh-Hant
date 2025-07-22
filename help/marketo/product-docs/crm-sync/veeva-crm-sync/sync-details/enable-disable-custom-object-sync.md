---
description: 啟用/停用自訂物件同步 — Marketo檔案 — 產品檔案
title: 啟用/停用自訂物件同步
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 啟用/停用自訂物件同步 {#enable-disable-custom-object-sync}

在您的[!DNL Veeva] CRM執行個體中建立的自訂物件也可以是Marketo Engage的一部分。 以下說明設定方法。

## 啟用或停用自訂物件同步 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**需要管理員許可權**

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**，然後按&#x200B;**[!UICONTROL Veeva Objects Sync]**。

   ![](assets/enable-disable-custom-object-sync-1.png)

1. 如果這是您的第一個自訂物件，請按一下&#x200B;**[!UICONTROL Sync Schema]**。 如果沒有，請按一下&#x200B;**[!UICONTROL Refresh Schema]**&#x200B;以確保您擁有最新版本。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. 如果您的全域同步正在執行，請按一下&#x200B;**[!UICONTROL Disable Global Sync]**&#x200B;以停用它。

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >同步[!DNL Veeva]自訂物件結構描述可能需要幾分鐘的時間。

1. 按一下「**[!UICONTROL Refresh Schema]**」。

   ![](assets/enable-disable-custom-object-sync-4.png)

選取您要同步的物件，然後按一下&#x200B;**[!UICONTROL Enable Sync]**。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo只有在[!DNL Veeva] CRM中與連絡人或帳戶物件有直接關係時，才能同步處理自訂物件。

1. 再按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 返回[!UICONTROL Veeva]標籤並按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/enable-disable-custom-object-sync-7.png)

## 使用您的自訂物件 {#using-your-custom-objects}

>[!NOTE]
>
>您無法在包含觸發器的智慧行銷活動中使用自訂物件。

1. 在您的[!UICONTROL Smart List]中，拖曳至&quot;**[!UICONTROL Has Opportunity]**&quot;篩選器並設為&#x200B;**[!UICONTROL True]**。

   ![](assets/enable-disable-custom-object-sync-8.png)

1. 或者，使用篩選條件限制來縮小焦點。

   ![](assets/enable-disable-custom-object-sync-9.png)

太好了！ 您現在可以在[!UICONTROL Smart Campaigns]和[!UICONTROL Smart Lists]中使用此自訂物件的資料。

>[!MORELIKETHIS]
>
>[新增/移除自訂物件欄位做為智慧列示/觸發條件約束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
