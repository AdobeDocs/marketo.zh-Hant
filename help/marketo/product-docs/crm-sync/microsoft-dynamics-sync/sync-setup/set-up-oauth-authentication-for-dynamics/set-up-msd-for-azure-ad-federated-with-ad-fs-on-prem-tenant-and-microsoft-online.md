---
description: 為Azure AD Federated設定MSD，並預裝AD FS、租用戶和Microsoft Online -Marketo文檔——產品文檔
title: 為Azure AD Federated設定MSD，並在On-prem、Tenant和Microsoft Online中設定AD FS
exl-id: b6c10048-d27e-4135-beef-232deddc2984
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 為Azure AD Federated設定MSD，並在{#set-up-msd-for-azure-ad-federated-with-ad-fs-on-prem-tenant-and-microsoft-online}上使用AD FS On-prem 、 Tenant和Microsoft Online

## 設定Microsoft Dynamics CRM應用程式{#set-up-microsoft-dynamics-crm-app}

1. 導覽至https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration。

1. 請遵循所有步驟。 在步驟3中，輸入相關應用程式名稱(例如「Marketo整合」)。 在「受支援的帳戶類型」下，選取「僅限此組織目錄中的帳戶」。

1. 記下應用程式ID(ClientId)。 你以後得進去Marketo。

1. 依照本文[中的步驟，授與管理員同意。](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md)

1. 按一下「憑證與機密」****，在管理中心產生「用戶端機密」。

   ![](assets/set-up-msd-for-azure-ad-federated-1.png)

1. 按一下「**新客戶機密碼**」。

   ![](assets/set-up-msd-for-azure-ad-federated-2.png)

1. 新增用戶端密碼說明，然後按一下&#x200B;**Add**。

   ![](assets/set-up-msd-for-azure-ad-federated-3.png)

   >[!CAUTION]
   >
   >請務必記下「用戶端密碼」值（如下方的螢幕擷取所示），因為您稍後會需要它。 它只顯示一次，您將無法再擷取它。

   ![](assets/set-up-msd-for-azure-ad-federated-4.png)

Marketo使用grant_type資源擁有者密碼憑證(ROPC)向OAuth驗證Azure廣告。 此方案需要為特定應用程式建立「主領域搜索」策略。 使用此策略，Azure AD會將驗證請求重新導向至聯合服務。 必須在AD Connect中為此啟用口令散列同步。 如需詳細資訊，請參閱[OAuth with ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)和[設定應用程式的hrd原則](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)。

其他參考[可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20astle%20includes%20federated,are%20federated%20to%20Azure%20AD。)。

完成後，您應將&#x200B;**輸入Dynamics CRM產生的用戶端Id和密碼至Marketo**。

## 將Dynamics CRM產生的用戶端Id和密碼輸入Marketo{#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

1. 在Marketo，按一下&#x200B;**管理**。

   ![](assets/set-up-msd-for-azure-ad-federated-5.png)

1. 按一下&#x200B;**Microsoft Dynamics**。

   ![](assets/set-up-msd-for-azure-ad-federated-6.png)

1. 按一下&#x200B;**禁用同步**。

   ![](assets/set-up-msd-for-azure-ad-federated-7.png)

1. 在憑據旁，按一下&#x200B;**編輯**。

   ![](assets/set-up-msd-for-azure-ad-federated-8.png)

1. 輸入先前檢索到的&#x200B;**客戶端ID**&#x200B;和&#x200B;**客戶端密碼** ，然後按&#x200B;**保存**。

   ![](assets/set-up-msd-for-azure-ad-federated-9.png)

1. 按一下&#x200B;**驗證同步設定**。

   ![](assets/set-up-msd-for-azure-ad-federated-10.png)

1. 按一下&#x200B;**Next**。

   ![](assets/set-up-msd-for-azure-ad-federated-11.png)

1. 您應看到所有綠色勾號。 按一下&#x200B;**關閉**。

   ![](assets/set-up-msd-for-azure-ad-federated-12.png)

   >[!NOTE]
   >
   >如果您在綠色核取標籤中看到紅色X，請參閱[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以取得修正選項。

1. 按一下&#x200B;**啟用同步**。

   ![](assets/set-up-msd-for-azure-ad-federated-13.png)

就這樣！
