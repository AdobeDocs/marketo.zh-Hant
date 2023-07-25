---
unique-page-id: 3571800
description: 步驟3之3 — 連線Marketo與Salesforce （專業） - Marketo檔案 — 產品檔案
title: 步驟3之3 — 連線Marketo和Salesforce （專業）
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 步驟3之3：連結Marketo和Salesforce （專業） {#step-of-connect-marketo-and-salesforce-professional}

在本文中，您將設定Marketo以與已設定的Salesforce執行個體同步。

>[!PREREQUISITES]
>
>* [步驟1/3：將Marketo欄位新增至Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [步驟2 （共3步）：建立Marketo的Salesforce使用者（專業）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

## 擷取同步處理使用者安全性權杖 {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已經有安全性權杖，請直接進入「設定同步使用者認證」和「榮譽」進行準備！

1. 使用Marketo同步使用者登入Salesforce，按一下同步使用者的名稱，然後 **我的設定**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. 在導覽搜尋列中，輸入「reset」並按一下 **重設我的安全性權杖**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 按一下 **重設安全性權杖**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   安全性權杖會透過電子郵件傳送給您。

## 設定同步使用者認證 {#set-sync-user-credentials}

1. 在Marketo中，前往 **管理員**，選取 **CRM**，然後按一下 **與同步 [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >請確定 [隱藏您不需要的所有欄位](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) 在Marketo中從同步使用者開啟，然後按一下 **同步欄位**. 按一下「同步欄位」後，使用者可以看到的所有欄位將會在Marketo中永久建立，且無法刪除。

1. 輸入在Salesforce設定的第2部分建立的Salesforce同步使用者認證([專業](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)， [企業](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 並按一下 **同步欄位**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Check **Sandbox** 如果您正在將Marketo沙箱同步至Salesforce沙箱。

1. 閱讀警告，然後按一下 **確認認證**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果您想檢視 [對應和自訂它們](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)，這是您執行此動作的唯一機會！ 按一下「開始Salesforce同步」之後，就會完成。

## 開始Salesforce同步 {#start-salesforce-sync}

1. 按一下 **開始Salesforce同步** 以開始永久性Marketo-Salesforce同步。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不會針對Salesforce同步處理或手動輸入潛在客戶時自動進行重複資料刪除。

1. 按一下 **開始同步**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的時間會依資料庫的大小和複雜度而有所不同。

## 驗證同步 {#verify-sync}

Marketo會在管理區域提供Salesforce同步的狀態訊息。 您可以按照以下步驟驗證同步處理是否正常運作。

1. 在Marketo中，按一下 **管理員**，則 **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步狀態會顯示在右上角。 它會顯示下列三個訊息之一： **上次同步時間**， **同步進行中**，或 **已失敗**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

哇，您剛剛完成設定Marketo其中一項最強大的功能，現在就開始！

>[!MORELIKETHIS]
>
>* [在SalesforceAppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Professional Edition中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
