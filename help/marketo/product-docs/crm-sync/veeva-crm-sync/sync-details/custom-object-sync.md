---
description: 自訂物件同步 — Marketo檔案 — 產品檔案
title: 自訂物件同步
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
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
>若要使用自訂物件，必須將其與Veeva CRM中的聯絡人或帳戶物件相關聯。

## 啟用自訂物件 {#enable-custom-object}

1. 在Marketo中，按一下&#x200B;**[!UICONTROL 管理員]**，然後按&#x200B;**[!UICONTROL Veeva物件同步]**。

   ![](assets/custom-object-sync-1.png)

1. 如果這是您的第一個自訂物件，請按一下&#x200B;**[!UICONTROL 同步結構描述]**。

   ![](assets/custom-object-sync-2.png)

1. 按一下&#x200B;**[!UICONTROL 停用全域同步處理]**。

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva自訂物件結構描述的初始同步處理可能需要幾分鐘的時間。

1. 將您要同步的自訂物件拖曳至畫布。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >自訂物件必須具有唯一的名稱。 Marketo不支援兩個名稱相同的不同自訂物件。

1. 按一下&#x200B;**[!UICONTROL 啟用同步]**。

   ![](assets/custom-object-sync-5.png)

1. 再按一下&#x200B;**[!UICONTROL 啟用同步]**。

   ![](assets/custom-object-sync-6.png)

1. 返回&#x200B;**[!UICONTROL Veeva]**&#x200B;標籤。

   ![](assets/custom-object-sync-7.png)

1. 按一下&#x200B;**[!UICONTROL 啟用同步]**。

   ![](assets/custom-object-sync-8.png)

1. 若要檢視您的所有Veeva自訂物件，請按一下&#x200B;**[!UICONTROL 管理員]**&#x200B;和&#x200B;**[!UICONTROL Veeva物件同步]**。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至標準實體（一至兩個層級）的自訂實體。

太好了！ 您現在可以在智慧行銷活動和智慧清單中使用來自此自訂物件的資料。

>[!MORELIKETHIS]
>
>* [正在同步通話和通話主要訊息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [新增/移除自訂物件欄位做為智慧列示/觸發條件約束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
