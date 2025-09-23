---
unique-page-id: 4719300
description: 新增/移除自訂物件欄位做為智慧清單/觸發條件約束 — Marketo檔案 — 產品檔案
title: 新增/移除自訂物件欄位做為智慧清單/觸發程序限制
exl-id: 639e73eb-9a8c-4b10-8e97-892abf5c5db0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 12%

---

# 新增/移除自訂物件欄位做為智慧清單/觸發程序限制 {#add-remove-custom-object-field-as-smart-list-trigger-constraints}

Marketo Engage可讓您對Salesforce自訂物件同步處理執行更細微的控制。 這可讓您選取可在自訂物件篩選器中作為限制條件的欄位，並在Smart Campaigns中將其用作觸發器。

>[!NOTE]
>
>**需要管理員許可權**

1. 按一下&#x200B;**[!UICONTROL Admin].**

   ![](assets/add-remove-custom-object-field-1.png)

1. 按一下&#x200B;**[!UICONTROL Admin]**，然後按&#x200B;**[!UICONTROL Salesforce Objects Sync].**

   ![](assets/image2015-12-11-15-3a11-3a41.png)

1. **[!UICONTROL Salesforce Objects Sync]**&#x200B;會顯示在左欄。

   ![](assets/image2015-12-11-15-3a15-3a15.png)

1. 選取您要修改的物件。

   ![](assets/image2014-12-10-13-3a10-3a11.png)

1. 按一下「**[!UICONTROL Edit Visible Fields]**」。

   >[!TIP]
   >
   >如果&#x200B;**[!UICONTROL Edit Visible Fields]**&#x200B;按鈕呈現灰色，表示物件目前正在智慧清單或智慧行銷活動中使用。 移除所有關聯以繼續。

   ![](assets/image2014-12-10-13-3a10-3a25.png)

1. 如果您的全域同步已啟用，請按一下&#x200B;**[!UICONTROL Disable Global Sync]**。

   ![](assets/image2014-12-10-13-3a10-3a36.png)

1. 勾選所需的篩選/觸發條件約束旁的方塊，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-10-13-3a10-3a47.png)

   >[!NOTE]
   >
   >依預設，選取所有欄位作為篩選條件上的限制。

1. 按一下&#x200B;**[!UICONTROL Fields]**&#x200B;標籤以確認您的變更。

   ![](assets/image2014-12-10-13-3a10-3a56.png)

   >[!NOTE]
   >
   >別忘了重新啟用您的全域同步處理！

現在，您的智慧列示和智慧行銷活動甚至擁有更多功能。

>[!MORELIKETHIS]
>
>[啟用/停用自訂物件同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-custom-object-sync.md){target="_blank"}
