---
description: 第3步（共3步） — 連接Marketo Engage和Veeva CRM -Marketo文檔 — 產品文檔
title: 第3步（共3步） — 連接Marketo Engage和Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# 第3步（共3步）:連接Marketo Engage和Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

在本文中，您將配置Marketo Engage以與已配置的Veeva CRM實例同步。 **您會在一些彈出窗口中看到Salesforce** 因為Veeva CRM是基於Salesforce平台構建的。

>[!PREREQUISITES]
>
>* [第1步（共3步）:將Marketo欄位添加到Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;
>* [第2步（共3步）:為Marketo建立Veeva用戶](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target=&quot;_blank&quot;


>[!IMPORTANT]
>
>一次只能將一個Marketo實例連接到Veeva CRM實例。

## 使用OAuth連接到Veeva CRM {#connect-to-veeva-crm-using-oauth}

1. 在Marketo，按一下 **管理**。 選擇 **CRM** 按一下 **與維娃同步**。

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >一定要 [隱藏所有不需要的欄位](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)按一下「同步欄位」前，從同步用戶在Marketo中的{target=&quot;_blank&quot;}。 按一下「同步欄位」後，用戶可以看到的所有欄位將永久建立在Marketo，且無法刪除。

1. 按一下 **使用Veeva登錄**。

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >如果正在將Marketo沙盒同步到Veeva CRM沙盒，請檢查沙盒。

1. 按一下 **確認憑據**。

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. 將顯示一個帶有Salesforce登錄頁的彈出窗口。 輸入「Marketo同步用戶」憑據，然後按一下 **登錄**。

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. 輸入您通過電子郵件（由Salesforce發送）收到的驗證代碼，然後按一下 **驗證**。

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 成功驗證後，訪問頁面將顯示請求訪問。 按一下 **允許**。

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 幾分鐘後，Marketo恩加將出現一個彈出窗口。 按一下 **確認憑據**。

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## 啟動Veeva同步 {#start-veeva-sync}

1. 按一下 **啟動Veeva同步** 開始持續的Marketo — 維娃CRM同步。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo不會針對Veeva CRM同步或您手動輸入銷售線索時自動消除重複。

1. 按一下 **啟動同步**。

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>完成初始同步的時間因資料庫的大小和複雜性而異。

## 驗證同步 {#verify-sync}

Marketo在「管理」區域提供Veeva CRM同步的狀態消息。 通過執行以下步驟，可以驗證同步是否正常工作。

1. 在Marketo，按一下 **管理**，則 **韋瓦**。

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同步狀態在右上角可見。 它將顯示以下三條資訊之一：上次同步、正在同步或失敗。

>[!MORELIKETHIS]
>
>[配置自定義對象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;
