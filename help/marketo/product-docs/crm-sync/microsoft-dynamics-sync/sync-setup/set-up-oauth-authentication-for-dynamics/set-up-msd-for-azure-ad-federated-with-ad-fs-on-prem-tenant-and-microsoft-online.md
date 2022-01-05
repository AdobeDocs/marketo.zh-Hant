---
description: 為Azure AD Federated設定MSD，內部部署AD FS、租用戶和Microsoft Online - Marketo文檔 — 產品文檔
title: 為Azure AD Federated設定MSD，並預裝AD FS、租用戶和Microsoft Online
exl-id: b6c10048-d27e-4135-beef-232deddc2984
source-git-commit: 91ce0914755b578c896996fae1805022cb11c438
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 為Azure AD Federated設定MSD，並預裝AD FS、租用戶和Microsoft Online {#set-up-msd-for-azure-ad-federated-with-ad-fs-on-prem-tenant-and-microsoft-online}

## 設定Microsoft Dynamics CRM應用程式 {#set-up-microsoft-dynamics-crm-app}

1. 導覽至https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration。

1. 請遵循所有步驟。 在步驟3中，輸入相關的應用程式名稱(例如「Marketo整合」)。 在「受支援的帳戶類型」下，僅選擇此組織目錄中的「帳戶」。

1. 記下應用程式ID(ClientId)。 你以後要進Marketo。

1. 依照 [這篇文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 按一下「 」，在管理中心產生用戶端密碼 **憑證與機密**.

   ![](assets/set-up-msd-for-azure-ad-federated-1.png)

1. 按一下 **新用戶端密碼**.

   ![](assets/set-up-msd-for-azure-ad-federated-2.png)

1. 新增用戶端密碼說明，然後按一下 **新增**.

   ![](assets/set-up-msd-for-azure-ad-federated-3.png)

   >[!CAUTION]
   >
   >請務必記下「用戶端密碼」值（請見下方螢幕擷取畫面），因為您稍後會需要它。 它只顯示一次，您將無法再擷取它。

   ![](assets/set-up-msd-for-azure-ad-federated-4.png)

Marketo使用grant_type資源擁有者密碼憑證(ROPC)驗證Azure AD（使用OAuth）。 此情形需要為特定應用程式建立家庭領域發現策略。 使用此策略，Azure AD將驗證請求重定向到聯合身份驗證服務。 必須在AD Connect中為此啟用密碼哈希同步。 如需詳細資訊，請參閱 [OAuth與ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [為應用程式設定hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他參考 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20ass%20includes%20federated,are%20federated%20to%20Azure%20AD。).

你完事了，該 **將Dynamics CRM產生的用戶端Id和密碼輸入Marketo**.

## 將Dynamics CRM產生的用戶端Id和密碼輸入Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

1. 在Marketo中，按一下 **管理**.

   ![](assets/set-up-msd-for-azure-ad-federated-5.png)

1. 按一下 **Microsoft Dynamics**.

   ![](assets/set-up-msd-for-azure-ad-federated-6.png)

1. 按一下 **禁用同步**.

   ![](assets/set-up-msd-for-azure-ad-federated-7.png)

1. 在憑證旁，按一下 **編輯**.

   ![](assets/set-up-msd-for-azure-ad-federated-8.png)

1. 輸入 **用戶端ID** 和 **用戶端密碼** 您之前擷取並按下 **儲存**.

   ![](assets/set-up-msd-for-azure-ad-federated-9.png)

1. 按一下 **驗證同步設定**.

   ![](assets/set-up-msd-for-azure-ad-federated-10.png)

1. 按一下 **下一個**.

   ![](assets/set-up-msd-for-azure-ad-federated-11.png)

1. 您應該會看到所有綠色勾號。 按一下 **關閉**.

   ![](assets/set-up-msd-for-azure-ad-federated-12.png)

   >[!NOTE]
   >
   >如果綠色勾號中出現紅色X，請參閱 [這篇文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) （修正選項）。

1. 按一下 **啟用同步**.

   ![](assets/set-up-msd-for-azure-ad-federated-13.png)

就這樣！
