---
unique-page-id: 3571827
description: 第2步（共3步） — 設定「Marketo解決方案」，使用伺服器到伺服器連接 — Marketo文檔 — 產品文檔
title: 第2步（共3步） — 設定具有伺服器到伺服器連接的Marketo解決方案
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 48b8289994e000eafd72982ac1b4a0a809b10bab
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# 第2步（共3步）:設定Marketo解決方案，使用伺服器到伺服器連接 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[第1步（共3步）:安裝Marketo解決方案，使用伺服器到伺服器連接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)

## 在Azure AD中建立客戶端應用程式 {#create-client-application-in-azure-ad}

1. 導航到 [Microsoft的文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration)。

1. 執行所有步驟。 對於步驟3，輸入相關應用程式名稱(如「Marketo整合」)。 在支援的帳戶類型下，選擇 **僅此組織目錄中的帳戶**。

1. 記下應用程式ID(ClientId)和租戶ID。 你以後得進Marketo。

1. 按照以下步驟授予管理員同意 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md)。

1. 在管理中心中通過按一下 **證書和機密**。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 按一下 **新客戶機密鑰** 按鈕

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. 輸入客戶機密碼描述，然後按一下 **添加**。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>請確保記下「客戶機密碼」值（見下面的螢幕截圖），因為您以後需要它。 它只顯示一次，您將無法再次檢索它。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## 在Microsoft建立應用程式用戶 {#create-application-user-in-microsoft}

1. 按照以下連結中的步驟操作 [在Microsoft設定應用程式用戶](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation)。

   >[!IMPORTANT]
   >
   >* 向應用程式用戶授予權限時，請確保將其分配給「Marketo同步用戶角色」。
   >* 從中記錄應用程式用戶的電子郵件地址 [查看詳細資訊選項](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) 在電源平台上。 在Marketo內設定與MS Dynamics的連接時，此電子郵件地址將用作用戶名。


## Azure AD Federated with AD FS On-prem {#azure-ad-federated-with-ad-fs-on-prem}

聯合Azure AD到ADFS Onprem需要為特定應用程式建立「主領域發現」策略。 使用此策略，Azure AD將將身份驗證請求重定向到聯合身份驗證服務。 必須在AD Connect中為此啟用密碼哈希同步。 有關詳細資訊，請參閱 [使用ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [為應用程式設定hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)。

其他引用 [可在此處找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20報表%20還%20包括%20聯合，%20聯合%20到%20Azure%20AD。)。

## 配置Marketo解決方案 {#configure-marketo-solution}

快到了！ 我們只剩下了通知Marketo解決方案部門有關新用戶建立的資訊。

>[!IMPORTANT]
>
>如果要從「基本身份驗證」升級到OAuth，則需要聯繫 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support) 的子菜單。 對預設同步用戶執行配置更改將暫時停止同步，直到輸入新憑據並重新啟用同步。 如果您要恢復到舊的身份驗證方法，Marketo支援可以禁用該功能（2022年4月之前）。

1. 返回「高級設定」部分，然後按一下 ![](assets/image2015-5-13-15-3a49-3a19.png) 表徵圖，然後選擇 **Marketo配置**。

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果你看不到 **Marketo配置** 在「設定」菜單中，刷新頁面。 如果這行不通，盡量 [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md) 或註銷並重新登錄。

1. 按一下 **預設**。

   ![](assets/fifteen.png)

1. 按一下 **Marketo用戶** 欄位，然後選擇您建立的同步用戶。

   ![](assets/sixteen.png)

1. 按一下 ![](assets/image2015-3-13-15-3a10-3a11.png) 按鈕，將選定控制項在Tab鍵次序中下移一個位置。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 按一下 **X** 的上界。

   ![](assets/seventeen.png)

1. 按一下 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 表徵圖，然後選擇 **解決方案**。

   ![](assets/eighteen.png)

1. 按一下 **發佈所有自定義項** 按鈕

   ![](assets/nineteen.png)

## 繼續步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步的記錄數， [設定自定義同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 現在。
* 運行 [驗證MicrosoftDynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 處理。 它驗證初始設定是否正確。
* 登錄到MarketoDynamics CRM中的Microsoft同步用戶。

>[!MORELIKETHIS]
>
>* [第3步（共3步）:將Marketo解決方案與伺服器連接連接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [重新配置Dynamics身份驗證方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)

