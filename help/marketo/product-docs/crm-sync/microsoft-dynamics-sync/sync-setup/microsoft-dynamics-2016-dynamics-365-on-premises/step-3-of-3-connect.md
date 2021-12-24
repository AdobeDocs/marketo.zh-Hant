---
description: Install Marketo for Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 3 of 3 - Marketo Docs - Product Documentation
title: 安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟3（共3步）
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Step 3 of 3: Connect Marketo Dynamics (2016 On Prem/Dynamics 365 On-Premises) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Install Marketo for Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 2 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**需要管理權限**

## 輸入Dynamics同步用戶資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo，然後按一下 **管理**.

   ![](assets/login-admin.png)

1. Click **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. 選擇 **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Click **Edit** in **Step 1: Enter Credentials**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >請確定您的憑證正確，因為提交後，我們無法還原後續的架構變更。 如果儲存的憑證不正確，您必須取得新的Marketo訂閱。

1. 輸入 **使用者名稱**, **密碼** a Microsoft Dynamics **URL**&#x200B;和 **用戶端Id/密碼**. Click **Save** when done.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 如果您的Marketo是在2020年10月之前布建，用戶端ID和密碼為選用欄位。 否則，它們是強制性的。 獲取此資訊取決於您使用的MSD版本。
   >* Marketo中的使用者名稱必須符合CRM中同步使用者的使用者名稱。 The format can be `user@domain.com` or DOMAIN\user.
   >* 如果您不知道URL, [在這裡了解如何找到](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


   >[!TIP]
   >
   >不知道URL? We will show you how to find your [Dynamics Organization Service URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) here.

## 選擇要同步的欄位 {#select-fields-to-sync}

1. Click **Edit** in **Step 2: Select Fields to Sync**.

   ![](assets/image2015-3-16-9-51-28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取這些欄位。 Click **Save**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [已禁用同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然後編輯並儲存Marketo中的結構，以重新整理 [選擇要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sync Fields for a Custom Filter {#sync-fields-for-a-custom-filter}

If you&#39;ve created a custom filter, be sure to go in and select the new fields to be synced with Marketo.

1. 前往「管理」並選取 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Click **Edit** on Field Sync Details.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 The actual name must be new_synctomkto but the Display Name can be anything. 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 啟用同步 {#enable-sync}

1. 按一下 **編輯** in **步驟3:啟用同步**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo will not automatically de-dupe against a Microsoft Dynamics sync, or when you manually enter people.

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下 **開始同步**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要數小時。 完成後，您會收到電子郵件通知。

   ![](assets/image2015-3-16-9-59-51.png)

幹得好！
