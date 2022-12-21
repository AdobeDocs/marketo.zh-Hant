---
unique-page-id: 3571827
description: 第2步（共3步） — 使用伺服器對伺服器連線設定Marketo解決方案 — Marketo檔案 — 產品檔案
title: 第2步（共3步） — 使用伺服器對伺服器連線設定Marketo解決方案
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 3a52db828a9bbf01b617d6e417d078d11ea30fb7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 第2步（共3步）:使用伺服器對伺服器連線設定Marketo解決方案 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[第1步（共3步）:安裝具有伺服器對伺服器連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)

## 在Azure AD中建立客戶端應用程式 {#create-client-application-in-azure-ad}

1. 導覽至 [這篇Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration).

1. 請遵循所有步驟。 在步驟3中，輸入相關的應用程式名稱(例如「Marketo整合」)。 在「支援的帳戶類型」下，選擇 **僅此組織目錄中的帳戶**.

1. 記下應用程式ID(ClientId)和租用戶ID。 你以後要進Marketo。

1. 依照下列步驟授與管理員同意 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 按一下「 」，在管理中心產生用戶端密碼 **憑證與機密**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 按一下 **新用戶端密碼** 按鈕。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. 輸入客戶端密碼說明，然後按一下 **新增**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>請務必記下「用戶端密碼」值（請見下方螢幕擷取畫面），因為您稍後會需要它。 它只顯示一次，您將無法再擷取它。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## 在Microsoft中建立應用程式使用者 {#create-application-user-in-microsoft}

1. 請依照下列連結中的步驟操作： [在Microsoft中設定應用程式使用者](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation).

   >[!IMPORTANT]
   >
   >* 授予應用程式使用者權限時，請務必將其指派給「Marketo同步使用者角色」。
   >* 請記下 [查看詳細資訊選項](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) 在Power Platform上。 在Marketo內設定與MS Dynamics的連線時，此電子郵件地址將會作為使用者名稱。


## Azure AD Federated與AD FS內部部署 {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD到ADFS Onprem需要為特定應用程式建立家庭領域發現策略。 使用此策略，Azure AD將驗證請求重定向到聯合身份驗證服務。 必須在AD Connect中為此啟用密碼哈希同步。 如需詳細資訊，請參閱 [OAuth與ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [為應用程式設定hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他參考 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20ass%20includes%20federated,are%20federated%20to%20Azure%20AD。).

## 設定Marketo解決方案 {#configure-marketo-solution}

快到了！ 我們只需將新使用者建立的相關資訊告知Marketo解決方案即可。

1. 返回「進階設定」區段，然後按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 表徵圖，然後選擇 **Marketo設定**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果你沒看到 **Marketo設定** 在「設定」功能表中，重新整理頁面。 如果那行不通，試試 [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md) 再次登出或重新登入。

1. 按一下 **預設**.

   ![](assets/fifteen.png)

1. 按一下 **Marketo使用者** 欄位，然後選取您建立的同步使用者。

   ![](assets/sixteen.png)

1. 按一下 ![](assets/image2015-3-13-15-3a10-3a11.png) 圖示以儲存變更。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下 **X** 在右上方以關閉畫面。

   ![](assets/seventeen.png)

1. 按一下 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 表徵圖，然後選擇 **解決方案**.

   ![](assets/eighteen.png)

1. 按一下 **發佈所有自訂** 按鈕。

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >如果您要從基本驗證升級為OAuth，可以使用 [這篇文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) 重新配置身份驗證。

## 繼續執行步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 現在。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它會驗證您的初始設定是否正確執行。
* 登入Microsoft Dynamics CRM中的Marketo同步使用者。

>[!MORELIKETHIS]
>
>* [第3步（共3步）:將Marketo解決方案與伺服器連線連線](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [重新配置Dynamics身份驗證方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)

