---
description: 第3步（共3步） — 連線Marketo Engage和Veva CRM - Marketo檔案 — 產品檔案
title: 第3步（共3步） — 連接Marketo Engage和Veva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# 第3步（共3步）:連接Marketo Engage和Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

在本文中，您會將Marketo Engage設定為與已設定的Veeva CRM例項同步。 **在一些快顯視窗中，您會看到Salesforce** 因為Veva CRM是建立在Salesforce平台上。

>[!PREREQUISITES]
>
>* [第1步（共3步）:將Marketo欄位新增至Veva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}
>* [第2步（共3步）:建立Marketo的Veeva使用者](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target=&quot;_blank&quot;}


>[!IMPORTANT]
>
>一次只能將一個Marketo執行個體連線至Veva CRM執行個體。

## 使用OAuth連線至Veeva CRM {#connect-to-veeva-crm-using-oauth}

1. 在Marketo中，按一下 **管理**. 選擇 **CRM** 按一下 **與Veeva同步**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >一定要 [隱藏所有不需要的欄位](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)按一下「同步欄位」前，從同步使用者取得Marketo中的{target=&quot;_blank&quot;}。 按一下「同步欄位」後，使用者可看見的所有欄位都會在Marketo中建立，且無法刪除。

1. 按一下 **使用Veeva登入**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >如果您正在將Marketo沙箱同步至Veva CRM沙箱，請核取沙箱。

1. 按一下 **確認憑證**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. 將顯示帶有Salesforce登入頁面的快顯視窗。 輸入您的「Marketo同步使用者」憑證，然後按一下 **登入**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. 輸入您通過電子郵件（由Salesforce發送）收到的驗證代碼，然後按一下 **驗證**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 成功驗證後，存取頁面會顯示請求存取。 按一下 **允許**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 幾分鐘後，快顯視窗就會出現在Marketo Engae中。 按一下 **確認憑證**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## 啟動Veeva同步 {#start-veeva-sync}

1. 按一下 **啟動Veeva同步** 開始持續的Marketo-Veeva CRM同步。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo不會針對Veva CRM同步或當您手動輸入銷售機會時自動刪除重複資料。

1. 按一下 **開始同步**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>完成初始同步的時間會根據資料庫的大小和複雜性而有所不同。

## 驗證同步 {#verify-sync}

Marketo會在「管理」區域中提供Veva CRM同步的狀態訊息。 您可以依照下列步驟來驗證同步是否正確運作。

1. 在Marketo中，按一下 **管理**，然後 **韋瓦**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同步狀態顯示在右上角。 它將顯示三條消息之一：上次同步、同步進行中或失敗。

>[!MORELIKETHIS]
>
>[配置自定義對象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}
