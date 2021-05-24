---
description: 設定Microsoft Dynamics CRM應用程式以進行線上 — Marketo檔案 — 產品檔案
title: 設定Microsoft Dynamics CRM應用程式以聯機
exl-id: ec3123c9-e484-4736-9831-9559cc393bd9
source-git-commit: 4283f1b6936316f3053543e06e7eaee45a7f2436
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 設定Microsoft Dynamics CRM應用程式以聯機{#set-up-microsoft-dynamics-crm-app-for-online}

## 設定{#set-up}

1. 導覽至https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration。

1. 請遵循所有步驟。 在步驟3中，輸入相關的應用程式名稱(例如「Marketo整合」)。 在「受支援的帳戶類型」下，僅選擇此組織目錄中的「帳戶」。

1. 記下應用程式ID(ClientId)。 你以後要進Marketo。

1. 依照本文章[中的步驟](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md)授予管理員同意。

1. 按一下&#x200B;**Certificates &amp; secrets**&#x200B;在管理中心產生用戶端密碼。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-1.png)

1. 按一下「**新增用戶端密碼**」。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-2.png)

1. 新增用戶端密碼說明，然後按一下&#x200B;**Add**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-3.png)

   >[!CAUTION]
   >
   >請務必記下「用戶端密碼」值（請見下方螢幕擷取畫面），因為您稍後會需要它。 它只顯示一次，您將無法再擷取它。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-4.png)

Marketo使用grant_type資源擁有者密碼憑證(ROPC)驗證Azure AD（使用OAuth）。 此情形需要為特定應用程式建立家庭領域發現策略。 使用此策略，Azure AD將驗證請求重定向到聯合身份驗證服務。 必須在AD Connect中為此啟用密碼哈希同步。 如需詳細資訊，請參閱[OAuth with ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)和[為應用程式](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)設定hrd原則。

您可在此處](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20ass%20includes%20federated,are%20federated%20to%20Azure%20AD。)找到其他參考[。

完成後，您可以在Marketo **中輸入Dynamics CRM產生的用戶端Id和密碼。**

## 在Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}中輸入Dynamics CRM產生的用戶端Id和密碼

下列步驟適用於線上&#x200B;_和_&#x200B;預先版本。

1. 在Marketo中，按一下&#x200B;**管理**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-5.png)

1. 按一下&#x200B;**Microsoft Dynamics**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-6.png)

1. 按一下「**禁用同步**」。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-7.png)

1. 在憑據旁，按一下&#x200B;**Edit**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-8.png)

1. 輸入先前檢索到的&#x200B;**客戶端ID**&#x200B;和&#x200B;**客戶端密碼**，然後按&#x200B;**保存**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-9.png)

1. 按一下&#x200B;**驗證同步設定**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-10.png)

1. 按一下&#x200B;**Next**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-11.png)

1. 您應該會看到所有綠色勾號。 按一下&#x200B;**關閉**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-12.png)

   >[!NOTE]
   >
   >如果綠色勾號中出現紅色X，請參閱[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以了解修正選項。

1. 按一下「**啟用同步**」。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-13.png)

就這樣！
