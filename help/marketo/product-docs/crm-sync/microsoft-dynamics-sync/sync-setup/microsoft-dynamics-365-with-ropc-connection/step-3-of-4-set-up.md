---
description: 步驟4之3 — 在MS Dynamics上設定使用者端應用程式 — Marketo檔案 — 產品檔案
title: 步驟4之3 — 在MS Dynamics上設定使用者端應用程式
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 步驟4之3：在MS Dynamics上設定使用者端應用程式 {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [步驟4：使用資源擁有者密碼控制連線安裝Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [步驟2/4：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)

1. 導覽至https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration。

1. 請依照所有步驟操作。 對於步驟3，請輸入相關的應用程式名稱(例如「Marketo整合」)。 在「支援的帳戶型別」下，選取「僅在此組織目錄中的帳戶」。

1. 寫下應用程式ID (ClientId)。 您稍後需要在Marketo中輸入。

1. 依照下列步驟授予管理員同意： [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 按一下「 」，在管理中心產生使用者端密碼 **憑證和密碼**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. 按一下 **新使用者端密碼**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. 新增使用者端密碼說明，然後按一下 **新增**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >請務必記下使用者端密碼值（見以下熒幕擷圖），因為您稍後會需要它。 它只會顯示一次，您將無法再次擷取。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated與AD FS內部部署 {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD至ADFS Onprem需要建立特定應用程式的主領域探索原則。 使用此原則時，Azure AD會將驗證要求重新導向至同盟服務。 您必須在AD Connect中啟用密碼雜湊同步處理，才能執行此作業。 如需詳細資訊，請參閱 [使用ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [設定應用程式的hrd原則](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他參考 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated，are%20federated%20to%20Azure%20AD。).

## 繼續進行步驟4之前 {#before-proceeding-to-step-4}

* 如果要限制同步處理的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 立即。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它可驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo Sync使用者。

>[!MORELIKETHIS]
>
>* [步驟4之4：使用資源擁有者密碼控制連線來連線Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md)
