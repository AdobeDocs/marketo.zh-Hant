---
unique-page-id: 4719297
description: 啟用／停用自訂物件同步-Marketo檔案——產品檔案
title: 啟用／停用自訂物件同步
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 啟用／禁用自定義對象同步{#enable-disable-custom-object-sync}

在Salesforce例項中建立的自訂物件也可以是Marketo的一部分。 這是如何設定的。

## 啟用／禁用自定義對象同步{#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>需要管理員權限。

1. 按一下&#x200B;**管理**。

   ![](assets/one.png)

1. 在「資料庫管理」菜單中，按一下&#x200B;**Salesforce對象同步**。

   ![](assets/two-2.png)

1. 如果這是您的第一個自定義對象，請按一下&#x200B;**同步模式。** 否則，請 **按一** 下「重新整理計畫」，確保您擁有最新版。

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. 如果全局同步正在運行，則必須按一下&#x200B;**禁用全局同步。**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >同步Salesforce自訂物件架構可能需要幾分鐘的時間。

1. 按一下&#x200B;**刷新方案**。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 選擇要同步的對象，然後按一下&#x200B;**啟用同步**。

   >[!TIP]
   >
   >Marketo只能在自訂物件與Salesforce中的Lead、Contact或Account物件有直接關係時，才能同步該物件。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 再次按一下&#x200B;**啟用同步**。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 返回&#x200B;**Salesforce**&#x200B;標籤，然後按一下「啟用同步」。****

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## 使用自訂物件{#using-your-custom-objects}

>[!NOTE]
>
>您無法在具有觸發器的智慧型促銷活動中使用自訂物件。

1. 在智慧清單中，拖動到&#x200B;**Has Opportunity**&#x200B;過濾器並設定為&#x200B;**true**。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 然後，使用濾鏡約束來縮小焦點。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   太棒了！ 您現在可以在智慧型促銷活動和智慧型清單中使用此自訂物件的資料。

>[!MORELIKETHIS]
>
>[將自定義對象欄位添加／刪除為智慧清單／觸發器約束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
