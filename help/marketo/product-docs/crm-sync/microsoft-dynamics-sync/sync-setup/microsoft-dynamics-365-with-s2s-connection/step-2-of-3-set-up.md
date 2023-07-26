---
unique-page-id: 3571827
description: 步驟3之2 — 設定具有伺服器對伺服器連線的Marketo解決方案 — Marketo檔案 — 產品檔案
title: 步驟3之2 — 設定具有伺服器對伺服器連線的Marketo解決方案
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# 步驟3之2：設定具有伺服器對伺服器連線的Marketo解決方案 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[步驟3之1：安裝具有伺服器對伺服器連線的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## 在Azure AD中建立使用者端應用程式 {#create-client-application-in-azure-ad}

1. 瀏覽至 [此Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. 請依照所有步驟操作。 在步驟3中，輸入相關的應用程式名稱(例如「Marketo整合」)。 在支援的帳戶型別下，選取 **僅此組織目錄中的帳戶**.

1. 寫下應用程式ID (ClientId)和租使用者ID。 您稍後需要在Marketo中輸入。

1. 依照下列步驟授予管理員同意 [本文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. 按一下「 」，在「管理中心」產生使用者端密碼 **憑證和密碼**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 按一下 **新使用者端密碼** 按鈕。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. 輸入使用者端密碼說明，然後按一下 **新增**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>請務必記下使用者端密碼值（請參見下面的熒幕擷圖），因為您稍後會需要它。 它只會顯示一次，您將無法再次擷取。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## 在Microsoft中建立應用程式使用者 {#create-application-user-in-microsoft}

1. 請依照下列連結中的步驟前往 [在Microsoft中設定應用程式使用者](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* 授與應用程式使用者的許可權時，請務必將其指派給「Marketo同步使用者角色」。
   >* 請注意，應用程式使用者的電子郵件地址 [檢視詳細資料選項](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} 在Power Platform上。 在Marketo中設定MS Dynamics連線時，此電子郵件地址會作為使用者名稱。
   >* 同步使用者在您的CRM中所做的任何更新都將 **非** 已同步回Marketo。

## Azure AD Federated與AD FS內部部署 {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD至ADFS Onprem需要為特定應用程式建立主領域探索原則。 使用此原則時，Azure AD會將驗證要求重新導向至同盟服務。 必須在AD Connect中啟用密碼雜湊同步處理。 如需詳細資訊，請參閱 [使用ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

其他參考資料 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20also%20include%20federated，為%20federated%20to%20Azure%20AD。){target="_blank"}.

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 我們只剩下通知Marketo解決方案有關建立的新使用者。

1. 返回「進階設定」區段，然後按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 圖示並選取「 」 **Marketo設定**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您沒有看到 **Marketo設定** 在「設定」功能表中，重新整理頁面。 如果這樣無法解決問題，請嘗試 [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} 再次登出並重新登入。

1. 按一下 **預設**.

   ![](assets/fifteen.png)

1. 按一下 **Marketo使用者** 欄位並選取您建立的同步使用者。

   ![](assets/sixteen.png)

1. 按一下 ![](assets/image2015-3-13-15-3a10-3a11.png) 圖示以儲存變更。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下 **X** 以關閉熒幕。

   ![](assets/seventeen.png)

1. 按一下 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 圖示並選取「 」 **解決方案**.

   ![](assets/eighteen.png)

1. 按一下 **發佈所有自訂** 按鈕。

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >如果您要從基本驗證升級為OAuth，您可以使用 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} 以重新設定驗證。

## 繼續進行步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步處理的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} 立即。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} 程式。 它可驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo Sync User。

>[!MORELIKETHIS]
>
>* [步驟3之3：使用伺服器對伺服器連線連線Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md){target="_blank"}
>* [重新設定Dynamics驗證方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
