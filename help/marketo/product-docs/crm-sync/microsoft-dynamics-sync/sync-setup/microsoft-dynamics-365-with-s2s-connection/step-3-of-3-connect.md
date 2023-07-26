---
unique-page-id: 3571830
description: 步驟3之3 — 將Marketo解決方案與伺服器連線至伺服器 — Marketo檔案 — 產品檔案
title: 步驟3之3 — 使用伺服器對伺服器連線連線Marketo解決方案
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# 步驟3之3：使用伺服器對伺服器連線連線Marketo解決方案 {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

這是同步的最後一個步驟。 我們即將完成！

>[!PREREQUISITES]
>
>* [步驟3之1：安裝具有伺服器對伺服器連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [步驟3之2：設定具有伺服器對伺服器連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)

>[!NOTE]
>
>**需要管理員許可權**

>[!IMPORTANT]
>
>如果您要從基本驗證升級為OAuth，您需要聯絡 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support) 以取得更新其他引數的說明。 啟用此功能將暫時停止同步，直到輸入新憑證並重新啟用同步為止。 如果您想要恢復為舊的驗證模式，可以停用該功能（直到2022年4月）。

>[!NOTE]
>
>輸入新認證之前，您可以 [在這裡驗證它們](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

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
   >請確認您的組織URL正確無誤，因為提交後即無法回覆後續的結構描述變更。 如果使用錯誤的組織URL，您必須取得新的Marketo訂閱。 如果您不知道URL， [在此處瞭解如何找到它](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. 輸入Dynamics Sync使用者資訊，然後按一下 **儲存** 完成時。

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Marketo中的使用者名稱必須符合 [電子郵件地址](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) CRM中的應用程式使用者身分。 格式可以是 `user@domain.com` 或DOMAIN\user。

## 選取要同步的欄位 {#select-fields-to-sync}

1. 按一下 **編輯** 在 **步驟2：選取要同步的欄位**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. 選取您要同步至Marketo的欄位，以便預先選取它們。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [同步已停用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Marketo接著，透過編輯並儲存 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## 自訂篩選器的同步欄位 {#sync-fields-for-a-custom-filter}

如果您已建立自訂篩選器，請務必前往並選取要與Marketo同步的新欄位。

1. 前往「管理員」並選取「 」 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **編輯** 欄位同步處理詳細資訊。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並進行核取。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## 啟用同步 {#enable-sync}

1. 按一下 **編輯** 在 **步驟3：啟用同步**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo不會針對Microsoft Dynamics同步處理或手動輸入人員或潛在客戶時，自動進行重複資料刪除。

1. 閱讀快顯視窗中的所有內容，輸入您的電子郵件地址，然後按一下 **開始同步**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. 第一次同步可能需要幾個小時。 完成後，您將會收到電子郵件通知。

   ![](assets/image2015-3-16-9-3a59-3a51.png)

做得很好！
