---
description: 步驟4之4 — 使用資源擁有者密碼控制連線來連線Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟4之4 — 使用資源擁有者密碼控制連線來連線Marketo解決方案
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 步驟4之4：使用資源擁有者密碼控制連線來連線Marketo解決方案 {#step-4-of-4-connect-the-marketo-solution-ropc}

這是同步的最後一個步驟。 您即將完成！

>[!PREREQUISITES]
>
>* [步驟4：使用資源擁有者密碼控制連線安裝Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [步驟2/4：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [步驟4之3：在MS Dynamics上設定使用者端應用程式](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>如果您要從基本驗證升級至OAuth，您可以使用 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) 以重新設定您的驗證。

## 輸入Dynamics同步使用者資訊 {#enter-dynamics-sync-user-information}

1. 登入Marketo並按一下 **管理員**.

   ![](assets/login-admin.png)

1. 按一下 **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. 選取 **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. 按一下 **編輯** 在 **步驟1：輸入認證**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >請確定您的組織URL正確，因為我們在提交後無法回覆後續的結構描述變更。 如果使用不正確的組織URL，您必須取得新的Marketo訂閱。 如果您不知道URL， [在此處瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!NOTE]
   >
   >輸入新認證之前，您可以 [在這裡驗證它們](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

1. 輸入 **使用者名稱**， **密碼**， Microsoft Dynamics **URL**， **使用者端ID**、和 **使用者端密碼**. 按一下 **儲存** 完成時。

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Marketo中的使用者名稱必須與CRM中同步使用者的使用者名稱相符。 格式可以是 `user@domain.com` 或DOMAIN\user。

## 選取要同步的欄位 {#select-fields-to-sync}

1. 按一下 **編輯** 在 **步驟2：選取要同步的欄位**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

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

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 啟用同步 {#enable-sync}

1. 按一下 **編輯** 在 **步驟3：啟用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步處理或手動輸入人員或潛在客戶時自動進行重複資料刪除。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件地址，然後按一下 **開始同步**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要幾個小時。 完成後，您將會收到電子郵件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

幹得好！

>[!MORELIKETHIS]
>
>[重新設定Dynamics驗證方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)