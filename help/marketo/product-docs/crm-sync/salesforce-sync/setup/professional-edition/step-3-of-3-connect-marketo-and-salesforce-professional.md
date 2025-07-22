---
unique-page-id: 3571800
description: 步驟3之3 — 連線Marketo與Salesforce （專業） - Marketo檔案 — 產品檔案
title: 步驟3之3 — 連線Marketo和Salesforce （專業）
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 步驟3之3：連線Marketo和[!DNL Salesforce] （專業） {#step-of-connect-marketo-and-salesforce-professional}

在本文中，您將設定Marketo Engage以與已設定的Salesforce執行個體同步。

>[!PREREQUISITES]
>
>* [步驟3之1：將Marketo欄位新增至Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [步驟2之3：為Marketo (Professional)建立Salesforce使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## 擷取同步處理使用者安全性權杖 {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已經有安全性權杖，請直接進入「設定同步使用者認證」和「稱號」進行準備！

1. 以Marketo Sync User登入Salesforce，按一下同步使用者名稱，然後按&#x200B;**[!UICONTROL My Settings]**。

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. 在導覽搜尋列中，輸入「reset」並按一下&#x200B;**[!UICONTROL Reset My Security Token]**。

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 按一下「**[!UICONTROL Reset Security Token]**」。

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   安全性權杖將會透過電子郵件傳送給您。

## 設定同步使用者認證 {#set-sync-user-credentials}

1. 在Marketo中，移至&#x200B;**[!UICONTROL Admin]**，選取&#x200B;**[!UICONTROL CRM]**，然後按一下&#x200B;**[!UICONTROL Sync with Salesforce.com]**。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >在按一下[之前，請務必](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"}隱藏Marketo中不需要的所有欄位&#x200B;**[!UICONTROL Sync Fields]**，不讓同步使用者看到。 按一下「同步欄位」後，使用者看見的所有欄位將會在Marketo中永久建立，且無法刪除。

1. 輸入在Salesforce組態第2部分建立的Salesforce同步使用者認證([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)， [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md))，然後按一下&#x200B;**[!UICONTROL Sync Fields]**。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >如果您正在將Marketo沙箱同步至Salesforce沙箱，請核取&#x200B;**[!UICONTROL Sandbox]**。

1. 閱讀警告，然後按一下&#x200B;**[!UICONTROL Confirm Credentials]**。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果您想檢視[對應並加以自訂](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}，這是您唯一的機會了！ 按一下「開始Salesforce同步」即可完成。

## 開始[!DNL Salesforce]同步 {#start-salesforce-sync}

1. 按一下&#x200B;**[!UICONTROL Start Salesforce Sync]**&#x200B;開始持續的Marketo-Salesforce同步處理。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不會針對[!DNL Salesforce]同步處理或手動輸入潛在客戶時，自動進行重複資料刪除。

1. 按一下「**[!UICONTROL Start Sync]**」。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的時間會因資料庫的大小和複雜度而有所不同。

## 驗證同步 {#verify-sync}

Marketo在管理區域提供[!DNL Salesforce]同步處理的狀態訊息。 您可以按照以下步驟驗證同步是否正常運作。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**，然後按&#x200B;**Salesforce**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步狀態會顯示在右上角。 它會顯示下列三個訊息之一： **[!UICONTROL Last Synced]**、**[!UICONTROL Sync in Progress]**&#x200B;或&#x200B;**[!UICONTROL Failed]**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

您剛剛完成設定Marketo其中一項最強大的功能，現在就開始！

>[!MORELIKETHIS]
>
>* [在Marketo AppExchange中安裝Salesforce Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [在Marketo Professional Edition中設定Salesforce Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
