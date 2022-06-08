---
unique-page-id: 2953471
description: SFDC同步 — 自定義對象同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 自定義對象同步
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# SFDC同步：自定義對象同步 {#sfdc-sync-custom-object-sync}

在Salesforce實例中建立的自定義對象也可以是Marketo的一部分。  下面是如何設定。

>[!NOTE]
>
>**需要管理權限**

>[!PREREQUISITES]
>
>要使用自定義對象，它必須與 [鉛](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)。 [聯繫](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)或 [帳戶](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) Salesforce中的對象。

## 啟用自定義對象  {#enable-custom-object}

1. 按一下 **管理** 和 **Salesforce對象同步** 的子菜單。

   ![](assets/image2015-11-19-10-3a28-3a5.png)。

1. 如果這是您的第一個自定義對象，請按一下 **同步架構**。

   ![](assets/rtaimage-2.png)

1. 按一下 **禁用全局同步**。

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce自定義對象架構的初始同步可能需要幾分鐘時間。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 將要同步的自定義對象拖到畫布中。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自定義對象必須具有唯一的名稱。 Marketo不支援兩個同名的不同自定義對象。

1. 按一下 **啟用同步**。

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 按一下 **啟用同步** 的雙曲餘切值。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >不要忘記重新啟用全局同步！

1. 返回 **Salesforce** 頁籤。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 按一下 **啟用同步**。

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 要查看所有Salesforce自定義對象，請按一下 **管理** 和 **Salesforce對象同步** 連結（與上面步驟1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo僅支援與標準實體連結的一個或兩個深度的定製實體。

### 下一步： {#whats-next}

[添加/刪除自定義對象欄位作為智慧清單/觸發器約束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

太棒了！ 您現在可以在智慧市場活動和智慧清單中使用此自定義對象的資料。
