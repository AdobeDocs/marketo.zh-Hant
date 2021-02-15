---
unique-page-id: 2360366
description: 第3步（共3步）- Connect Marketo和Salesforce（企業版／無限製版）-行銷人員檔案——產品檔案
title: 第3步（共3步）-將行銷人員連線至Salesforce（企業版／無限製版）
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---


# 步驟3（共3步）:將Marketo與Salesforce（企業／無限制）連接{#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

在本文中，您將設定Marketo與您設定的Salesforce例項同步。

>[!PREREQUISITES]
>
>* [步驟1（共3步）:將行銷人員欄位新增至Salesforce（企業版／無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [步驟2（共3步）:建立適用於行銷人員的Salesforce使用者（企業版／不限數量）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## 擷取同步使用者安全性Token {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已擁有安全性Token，請直接前往「設定同步使用者憑證」和「kudos」進行準備！

1. 使用Marketo Sync使用者登入Salesforce，按一下同步使用者的名稱，然後按一下「我的設定」**。**

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. 在快速查找中，鍵入&quot;reset&quot;並按一下&#x200B;**Reset My Security Token**。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 按一下「重設安全性Token」。****

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   安全性Token將會以電子郵件寄送給您。

## 設定同步用戶憑據{#set-sync-user-credentials}

1. 在Marketo中，前往&#x200B;**Admin**，選擇&#x200B;**CRM**，然後按一下「與[Salesforce.com](https://Salesforce.com)**同步」**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >請務必在按一下「同步欄位&#x200B;****」之前，先隱藏Marketo中不需要的所有欄位。 [](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md)按一下「同步欄位」後，使用者可看見的所有欄位將會在Market中永久建立，且無法刪除。

1. 輸入在Salesforce設定第2部分([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)、[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md))中建立的Salesforce同步使用者憑證，然後按一下「同步欄位&#x200B;**」。**

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >如果您要將Marketo沙盒同步至Salesforce沙盒，請勾選&#x200B;**沙盒**。

1. 閱讀警告，然後按一下「確認認證&#x200B;**」。**

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果您想要查看[映射並自定義它們](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)，這是您唯一這樣做的機會！ 按一下「開始Salesforce同步」後，就完成。

## 啟動Salesforce同步{#start-salesforce-sync}

1. 按一下「啟動Salesforce Sync **」以開始持續的Marketo-Salesforce同步。**

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不會針對Salesforce同步或當您手動輸入銷售機會時自動消除重複資料。

1. 按一下&#x200B;**開始同步**。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的時間視資料庫的大小和複雜性而定。

## 驗證同步{#verify-sync}

Marketo在「管理」區域中提供Salesforce同步的狀態訊息。 您可以遵循下列步驟來驗證同步是否正常運作。

1. 在Marketo中，按一下&#x200B;**Admin**，然後按一下&#x200B;**Salesforce**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步狀態顯示在右上角。 它將顯示以下三條消息之一：**上次同步**、**正在同步**&#x200B;或&#x200B;**失敗**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

哇，您剛剛完成Marketo最強大功能之一的設定，您就去！

>[!MORELIKETHIS]
>
>* [步驟1（共3步）:將行銷人員欄位新增至Salesforce（企業版／無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [步驟2（共3步）:建立適用於行銷人員的Salesforce使用者（企業版／不限數量）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在Salesforce AppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Enterprise中設定Marketo Sales Insight/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

