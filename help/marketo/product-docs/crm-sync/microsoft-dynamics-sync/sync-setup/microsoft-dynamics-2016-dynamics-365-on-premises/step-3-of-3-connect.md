---
description: 安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟3之3 - Marketo檔案 — 產品檔案
title: 安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟3之3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 步驟3之3：連線Marketo Dynamics （2016在Prem/Dynamics 365內部部署） {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟2之3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)

>[!NOTE]
>
>**需要管理員許可權**

## 輸入Dynamics同步使用者資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo並按一下 **管理員**.

   ![](assets/login-admin.png)

1. 按一下 **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. 選取 **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. 按一下 **編輯** 在 **步驟1：輸入認證**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >請確認您的認證正確無誤，因為提交後無法回覆後續的結構描述變更。 如果儲存了不正確的認證，您必須取得新的Marketo訂閱。

1. 輸入 **使用者名稱**， **密碼** Microsoft Dynamics **URL**，和 **使用者端ID/密碼**. 按一下 **儲存** 完成時。

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* 如果您的Marketo是在2020年10月之前布建，則使用者端ID和密碼為選用欄位。 否則，它們是強制性的。 是否取得此資訊將取決於您使用的MSD版本。
   >* Marketo中的使用者名稱必須與CRM中同步使用者的使用者名稱相符。 格式可以是 `user@domain.com` 或DOMAIN\user。
   >* 如果您不知道URL， [在此處瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!TIP]
   >
   >不知道URL？ 我們將向您說明如何找到您的 [動態組織服務URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) 此處。

## 選取要同步的欄位 {#select-fields-to-sync}

1. 按一下 **編輯** 在 **步驟2：選取要同步的欄位**.

   ![](assets/image2015-3-16-9-51-28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [同步已停用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然後編輯並儲存，重新整理Marketo中的結構描述 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## 同步自訂篩選器的欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選取「 」 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **編輯** 欄位同步詳細資訊。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並勾選它。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## 啟用同步 {#enable-sync}

1. 按一下 **編輯** 在 **步驟3：啟用同步**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步處理或手動輸入人員時自動進行重複資料刪除。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件，然後按一下 **開始同步**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. 第一次同步可能需要幾個小時。 完成後，您將會收到電子郵件通知。

   ![](assets/image2015-3-16-9-59-51.png)

幹得好！
