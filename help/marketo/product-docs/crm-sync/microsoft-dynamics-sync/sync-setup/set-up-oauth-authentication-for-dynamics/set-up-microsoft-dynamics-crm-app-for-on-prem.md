---
description: 設定Microsoft Dynamics CRM應用程式以進行上市——行銷檔案——產品檔案
title: 設定Microsoft Dynamics CRM應用程式以進行預備
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# 針對On-prem {#set-up-microsoft-dynamics-crm-app-for-on-prem}設定Microsoft Dynamics CRM應用程式

Marketo中的用戶端ID/用戶端密碼設定可針對AD FS的隨選進行。 2016年或更新版本)。 若是舊版的On-prem，請聯絡[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)，以取得僅依據使用者ID和密碼而變更的驗證方法。

## 設定Microsoft Dynamics CRM應用程式{#set-up-microsoft-dynamics-crm-app}

請遵循[本Microsoft文章](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later)中的步驟。

完成後，下一步是&#x200B;**將Dynamics CRM產生的用戶端Id和密碼輸入Marketo**。

## 在Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}中輸入Dynamics CRM產生的用戶端Id和密碼

下列步驟適用於線上和上一版。

1. 在Marketo中，按一下&#x200B;**管理**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. 按一下&#x200B;**Microsoft Dynamics**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. 按一下&#x200B;**禁用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. 在憑據旁，按一下&#x200B;**編輯**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. 輸入先前檢索到的&#x200B;**客戶端ID**&#x200B;和&#x200B;**客戶端密碼** ，然後按&#x200B;**保存**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. 按一下&#x200B;**驗證同步設定**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. 按一下&#x200B;**Next**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. 您應看到所有綠色勾號。 按一下&#x200B;**關閉**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >如果您在綠色核取標籤中看到紅色X，請參閱[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以取得修正選項。

1. 按一下&#x200B;**啟用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

就這樣！
