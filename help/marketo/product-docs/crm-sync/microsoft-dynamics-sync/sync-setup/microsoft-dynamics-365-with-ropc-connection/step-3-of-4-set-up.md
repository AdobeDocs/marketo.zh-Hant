---
description: 第3步（共4步） — 在MS Dynamics上設定用戶端應用程式 — Marketo檔案 — 產品檔案
title: 第3步（共4步） — 在MS Dynamics上設定用戶端應用程式
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
source-git-commit: 0b9a1f50d8828acf019c5c4f82021d327f396fca
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 第3步，共4步：在MS Dynamics上設定客戶端應用 {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [第1步，共4步：安裝具有資源擁有者密碼控制連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [第2步，共4步：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. 導覽至https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration。

1. 請遵循所有步驟。 在步驟3中，輸入相關的應用程式名稱(例如「Marketo整合」)。 在「受支援的帳戶類型」下，僅選擇此組織目錄中的「帳戶」。

1. 記下應用程式ID(ClientId)。 你以後要進Marketo。

1. 依照 [這篇文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 按一下「 」，在管理中心產生用戶端密碼 **憑證與機密**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. 按一下 **新用戶端密碼**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. 新增用戶端密碼說明，然後按一下 **新增**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >請務必記下「用戶端密碼」值（請見下方螢幕擷取畫面），因為您稍後會需要它。 它只顯示一次，您將無法再擷取它。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated與AD FS內部部署 {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD到ADFS Onprem需要為特定應用程式建立家庭領域發現策略。 使用此策略，Azure AD將驗證請求重定向到聯合身份驗證服務。 必須在AD Connect中為此啟用密碼哈希同步。 如需詳細資訊，請參閱 [OAuth與ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [為應用程式設定hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他參考 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20ass%20includes%20federated,are%20federated%20to%20Azure%20AD。).

## 繼續執行步驟4之前 {#before-proceeding-to-step-4}

* 如果要限制同步的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 現在。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它會驗證您的初始設定是否正確執行。
* 登入Microsoft Dynamics CRM中的Marketo同步使用者。

>[!MORELIKETHIS]
>
>* [第4步，共4步：將Marketo解決方案與資源擁有者密碼控制連線連線](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md)

