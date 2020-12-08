---
unique-page-id: 3571800
description: 第3步（共3步）- Connect Marketo和Salesforce（專業版）- Marketo Docs —— 產品檔案
title: 第3步（共3步）-將行銷人員與Salesforce（專業人員）連接
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# 步驟3（共3步）:將行銷人員與Salesforce（專業版）連結 {#step-of-connect-marketo-and-salesforce-professional}

在本文中，您將設定Marketo與您設定的Salesforce例項同步。

>[!NOTE]
>
>**必要條件**
>
>* [步驟1（共3步）:將行銷人員欄位新增至Salesforce（專業版）](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [步驟2（共3步）:建立適用於行銷人員的Salesforce使用者（專業版）](step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

>



## 擷取同步使用者安全性Token {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已擁有安全性Token，請直接前往「設定同步使用者憑證」和「kudos」進行準備！

1. 使用Marketo Sync使用者登入Salesforce，按一下同步使用者的名稱，然後按一下「我的 **設定」**。

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. 在導覽搜尋列中，輸入「reset」，然後按一下「 **Reset My Security Token」**。

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 按一 **下重設安全性Token**。

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   安全性Token會以電子郵件寄送給您。

## 設定同步用戶憑據 {#set-sync-user-credentials}

1. 在Marketo中，前往 **Admin**，選取 **CRM**，然後按一下「與 **[Salesforce.com同步」](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >在按一下「 [同步欄位」前](../../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) ，請務必先隱藏Marketto中不需要的所有欄位 ****。 按一下「同步欄位」後，使用者可看見的所有欄位將會在Market中永久建立，且無法刪除。

1. 輸入在Salesforce設定([Professional](https://community.marketo.com/MarketoArticle?id=kA050000000LJ3QCAW)、 [Enterprise](https://community.marketo.com/MarketoArticle?id=kA050000000LIwKCAW))第2部分中建立的Salesforce Sync使用者憑證，然後按一下「 **同步欄位**」。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >如果您 **要將Marketo Sandbox同步至Salesforce Sandbox，請勾選「沙箱** 」。

1. 閱讀警告，然後按一下「確 **認認證」**。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果您想要檢視映射並 [自訂它們](../../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)，這是您唯一的機會！ 按一下「開始Salesforce同步」後，就完成。

## 啟動Salesforce同步 {#start-salesforce-sync}

1. 按一 **下「啟動Salesforce同步** 」，開始持續的Marketo-Salesforce同步。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不會針對Salesforce同步或當您手動輸入銷售機會時自動消除重複資料。

1. 按一下 **開始同步**。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的時間視資料庫的大小和複雜性而定。

## 驗證同步 {#verify-sync}

Marketo在「管理」區域中提供Salesforce同步的狀態訊息。 您可以遵循下列步驟來驗證同步是否正常運作。

1. 在Marketo中，按一下「管 **理」**，然 **後按Salesforce**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步狀態顯示在右上角。 它將顯示以下三條消息之一： **上次同步**、 **正在同步或**&#x200B;失敗 ****。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

哇，您剛剛完成Marketo最強大功能之一的設定，您就去！

>[!NOTE]
>
>**相關文章**
>
>* [在Salesforce AppExchange中安裝Marketo Sales Insight套件](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Professional Edition中設定Marketo Sales Insight](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>* [可選步驟](http://docs.marketo.com/display/docs/optional+steps)

>



