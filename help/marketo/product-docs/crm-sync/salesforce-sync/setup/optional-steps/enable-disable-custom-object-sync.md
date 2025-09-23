---
unique-page-id: 4719297
description: 啟用/停用自訂物件同步 — Marketo檔案 — 產品檔案
title: 啟用/停用自訂物件同步
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 10%

---

# 啟用/停用自訂物件同步 {#enable-disable-custom-object-sync}

在Salesforce例項中建立的自訂物件也能成為Marketo Engage的一部分。 以下說明設定方法。

## 啟用/停用自訂物件同步 {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**需要管理員許可權**

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/enable-disable-custom-object-sync-1.png)

1. 在[資料庫管理]功能表中，按一下&#x200B;**[!UICONTROL Salesforce Objects Sync]**。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. 如果這是您的第一個自訂物件，請按一下&#x200B;**[!UICONTROL Sync schema]**。 否則，請按一下&#x200B;**[!UICONTROL Refresh Schema]**&#x200B;以確保您擁有最新版本。

   ![](assets/enable-disable-custom-object-sync-3.png)

1. 如果您正在執行全域同步處理，您必須按一下&#x200B;**[!UICONTROL Disable Global Sync]**&#x200B;以停用它。

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >同步[!DNL Salesforce]自訂物件結構描述可能需要幾分鐘的時間。

1. 按一下「**[!UICONTROL Refresh Schema]**」。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 選取您要同步的物件，然後按一下&#x200B;**[!UICONTROL Enable Sync]**。

   >[!TIP]
   >
   >如果Marketo與[!DNL Salesforce]中的潛在客戶、連絡人或帳戶物件有直接關係，則只能同步處理自訂物件。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 再按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 返回&#x200B;**[!DNL Salesforce]**&#x200B;標籤並按一下&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## 使用您的自訂物件 {#using-your-custom-objects}

>[!NOTE]
>
>您無法在Smart Campaigns中搭配觸發器使用自訂物件。

1. 在您的智慧清單中，拖曳至&#x200B;**[!UICONTROL Has Opportunity]**&#x200B;篩選器並設為&#x200B;**[!UICONTROL true]**。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 然後，使用篩選條件限制來縮小焦點。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   太好了！ 您現在可以在智慧行銷活動和智慧清單中使用此自訂物件的資料。

>[!MORELIKETHIS]
>
>[新增/移除自訂物件欄位做為智慧列示/觸發條件約束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
