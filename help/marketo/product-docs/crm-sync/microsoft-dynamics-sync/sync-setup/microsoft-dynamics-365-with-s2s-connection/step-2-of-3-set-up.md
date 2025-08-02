---
unique-page-id: 3571827
description: 步驟3之2 — 設定具有伺服器對伺服器連線的Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟3之2 — 設定具有伺服器對伺服器連線的Marketo解決方案
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 步驟3之2：設定具有伺服器對伺服器連線的Marketo解決方案 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[步驟3之1：安裝具有伺服器對伺服器連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## 建立使用者端應用程式於[!DNL Azure AD] {#create-client-application-in-azure-ad}

1. 瀏覽至[此Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}。

1. 請依照所有步驟操作。 在步驟3中，輸入相關的應用程式名稱（例如&quot;[!DNL Marketo Integration]&quot;）。 在支援的帳戶型別下，選取&#x200B;**僅在此組織目錄中的帳戶**。

1. 寫下應用程式ID (ClientId)和租使用者ID。 您稍後需要在Marketo中輸入。

1. 請依照本文章[中的步驟](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}授與管理員同意。

1. 按一下&#x200B;**[!UICONTROL Certificates & secrets]**&#x200B;在管理中心產生使用者端密碼。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 按一下&#x200B;**[!UICONTROL New client secret]**&#x200B;按鈕。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. 輸入使用者端密碼描述，然後按一下&#x200B;**[!UICONTROL Add]**。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>請務必記下使用者端密碼值（請參見下面的熒幕擷圖），因為您稍後會需要它。 它只會顯示一次，您將無法再次擷取。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## 在Microsoft中建立應用程式使用者 {#create-application-user-in-microsoft}

1. 請依照下列連結中的步驟操作，[在Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}中設定應用程式使用者。

   >[!IMPORTANT]
   >
   >* 授與應用程式使用者的許可權時，請務必將其指派給「Marketo同步使用者角色」。
   >* 記下Power Platform上[檢視詳細資料選項](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user)中的應用程式使用者電子郵件地址。 在Marketo中設定MS [!DNL Dynamics]的連線時，此電子郵件地址會作為使用者名稱。

## [!DNL Azure AD]與[!DNL AD FS On-prem]同盟 {#azure-ad-federated-with-ad-fs-on-prem}

同盟[!DNL Azure AD]至[!DNL ADFS Onprem]需要為特定應用程式建立主領域探索原則。 使用此原則，[!DNL Azure AD]會將驗證要求重新導向至同盟服務。 必須在[!DNL AD Connect]中為此啟用密碼雜湊同步處理。 如需詳細資訊，請參閱[[!DNL OAuth] 搭配 [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)和[為應用程式設定hrd原則](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)。

其他參考[可以在這裡找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=此%20report%20also%20include%20federated，為%20federated%20to%20Azure%20AD。){target="_blank"}。

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 我們只剩下通知Marketo解決方案有關建立的新使用者。

1. 返回[!UICONTROL Advanced Settings]區段並按一下![](assets/image2015-5-13-15-3a49-3a19.png)旁的[!UICONTROL Settings]圖示，然後選取&#x200B;**[!UICONTROL Marketo Config]**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您在「設定」功能表中看不到「Marketo設定」，請重新整理頁面。 如果仍無法解決問題，請再試一次[發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}，或登出再重新登入。

1. 按一下「**[!UICONTROL Default]**」。

   ![](assets/fifteen.png)

1. 按一下「**[!UICONTROL Marketo User]**」欄位上的「搜尋」按鈕，然後選取您建立的同步使用者。

   ![](assets/sixteen.png)

1. 按一下右下角的![](assets/image2015-3-13-15-3a10-3a11.png)圖示以儲存變更。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下右上角的&#x200B;**X**&#x200B;以關閉熒幕。

   ![](assets/seventeen.png)

1. 按一下![](assets/image2015-5-13-15-3a49-3a19-1.png)旁的[!UICONTROL Settings]圖示，然後選取&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/eighteen.png)

1. 按一下&#x200B;**[!UICONTROL Publish All Customizations]**&#x200B;按鈕。

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >如果您正在從基本驗證升級為[!DNL OAuth]，您可以使用[本文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)來重新設定您的驗證。

## 繼續進行步驟3之前 {#before-proceeding-to-step}

* 若要限制同步處理的記錄數目，請立即[設定自訂同步處理篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 執行[驗證 [!DNL Microsoft Dynamics] 同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)程式。 它可驗證您的初始設定是否正確完成。
* 在[!DNL Microsoft Dynamics] CRM中登入Marketo Sync User。

>[!MORELIKETHIS]
>
>* [步驟3之3：使用伺服器至伺服器連線來連線Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [重新設定 [!DNL Dynamics] 驗證方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
