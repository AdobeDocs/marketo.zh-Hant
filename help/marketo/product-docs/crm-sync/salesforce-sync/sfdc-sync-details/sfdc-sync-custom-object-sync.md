---
unique-page-id: 2953471
description: SFDC同步 — 自訂物件同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 自定義對象同步
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: 79cfb0396f690a370cdce4e4df3a23c7439c252e
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# SFDC同步：自訂物件同步 {#sfdc-sync-custom-object-sync}

在Salesforce例項中建立的自訂物件也可以是Marketo的一部分。  下面是如何設定它。

>[!NOTE]
>
>**需要管理權限**

>[!PREREQUISITES]
>
>若要使用自訂物件，它必須與 [銷售機會](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [聯絡人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)，或 [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) 對象。

>[!IMPORTANT]
>
>Marketo同步使用者需要自訂物件的讀取存取權，才能列出該物件並在其上執行同步。

## 啟用自訂物件  {#enable-custom-object}

1. 按一下 **管理** 和 **Salesforce對象同步** 連結。

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. 如果這是您的第一個自訂物件，請按一下 **同步架構**.

   ![](assets/rtaimage-2.png)

1. 按一下 **禁用全局同步**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce自訂物件架構的初始同步可能需要幾分鐘的時間。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 將您要同步的自訂物件拖曳至畫布中。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自訂物件的名稱必須是唯一的。 Marketo不支援兩個名稱相同的不同自訂物件。

1. 按一下 **啟用同步**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 按一下 **啟用同步** 。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >別忘了重新啟用全局同步！

1. 返回 **Salesforce** 標籤。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 按一下 **啟用同步**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 要查看所有Salesforce自定義對象，請按一下 **管理** 和 **Salesforce對象同步** 連結（與上述步驟1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至一或兩層深之標準實體的自訂實體。

### 接下來要做什麼： {#whats-next}

[將自定義對象欄位添加/刪除為智慧清單/觸發器約束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

太棒了！ 您現在可以在智慧型行銷活動和智慧清單中使用此自訂物件的資料。
