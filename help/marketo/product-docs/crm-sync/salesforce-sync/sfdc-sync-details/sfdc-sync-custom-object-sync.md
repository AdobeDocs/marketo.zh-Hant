---
unique-page-id: 2953471
description: SFDC同步 — 自訂物件同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 自訂物件同步
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# SFDC同步：自訂物件同步 {#sfdc-sync-custom-object-sync}

在Salesforce例項中建立的自訂物件也可以是Marketo Engage的一部分。 以下說明設定方法。

>[!NOTE]
>
>**需要管理員許可權**

>[!PREREQUISITES]
>
>若要使用自訂物件，必須將其關聯至 [銷售機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}, or [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"} Salesforce中的物件。

>[!IMPORTANT]
>
>Marketo同步使用者需要自訂物件的讀取存取權，才能列出該物件並對其執行同步。

## 啟用自訂物件  {#enable-custom-object}

1. 按一下 **[!UICONTROL 管理員]** 和 **[!UICONTROL Salesforce物件同步]** 連結。

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. 如果這是您的第一個自訂物件，請按一下 **[!UICONTROL 同步結構描述]**.

   ![](assets/rtaimage-2.png)

1. 按一下 **[!UICONTROL 停用全域同步]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce自訂物件結構描述的初始同步可能需要幾分鐘的時間。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 將您要同步的自訂物件拖曳至畫布。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自訂物件必須具有唯一的名稱。 Marketo不支援兩個名稱相同的不同自訂物件。

1. 按一下 **[!UICONTROL 啟用同步]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 按一下 **[!UICONTROL 啟用同步]** 再來一次。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >別忘了重新啟用您的全域同步處理！

1. 返回 **Salesforce** 標籤。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 按一下 **[!UICONTROL 啟用同步]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 若要檢視所有Salesforce自訂物件，請按一下 **[!UICONTROL 管理員]** 和 **[!UICONTROL Salesforce物件同步]** 連結（與前述步驟1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至標準實體（一或兩個層級）的自訂實體。

### 下一步： {#whats-next}

[新增/移除自訂物件欄位做為智慧清單/觸發條件約束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

太好了！ 您現在可以在智慧行銷活動和智慧清單中使用來自此自訂物件的資料。
