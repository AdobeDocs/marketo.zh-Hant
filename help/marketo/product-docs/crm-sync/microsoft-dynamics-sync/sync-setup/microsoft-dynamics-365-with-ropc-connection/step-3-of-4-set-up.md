---
description: 步驟4之3 — 在MS Dynamics上設定使用者端應用程式 — Marketo檔案 — 產品檔案
title: 步驟4之3 — 在MS Dynamics上設定使用者端應用程式
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 步驟4之3：在MS Dynamics上設定使用者端應用程式 {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [步驟4之1：安裝具有資源擁有者密碼控制連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [步驟4之2：使用資源擁有者密碼控制連線設定Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. 瀏覽至此 [Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. 請依照所有步驟操作。 在步驟3中，輸入相關的應用程式名稱(例如「Marketo整合」)。 在支援的帳戶型別下，選取僅在此組織目錄中的帳戶。

1. 寫下應用程式ID (ClientId)。 您稍後需要在Marketo中輸入。

1. 請依照下列步驟授予管理員同意： [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. 按一下「 」，在「管理中心」產生使用者端密碼 **[!UICONTROL 憑證和密碼]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. 按一下 **[!UICONTROL 新使用者端密碼]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. 新增使用者端密碼說明，然後按一下 **[!UICONTROL 新增]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >請務必記下使用者端密碼值（請參見下面的熒幕擷圖），因為您稍後會需要它。 它只會顯示一次，您將無法再次擷取。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated與AD FS內部部署 {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD至ADFS Onprem需要為特定應用程式建立主領域探索原則。 使用此原則時，Azure AD會將驗證要求重新導向至同盟服務。 必須在AD Connect中啟用密碼雜湊同步處理。 如需詳細資訊，請參閱 [使用ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

其他參考資料 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20also%20include%20federated，為%20federated%20to%20Azure%20AD。){target="_blank"}.

## 繼續進行步驟4之前 {#before-proceeding-to-step-4}

* 如果要限制同步處理的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} 立即。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} 程式。 它可驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo Sync User。

>[!MORELIKETHIS]
>
>* [步驟4之4：使用資源擁有者密碼控制連線來連線Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
