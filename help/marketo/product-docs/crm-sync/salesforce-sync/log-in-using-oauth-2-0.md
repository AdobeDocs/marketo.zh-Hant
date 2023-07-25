---
description: 使用OAuth 2.0登入 — Marketo檔案 — 產品檔案
title: 使用OAuth 2.0登入
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 使用OAuth 2.0登入 {#log-in-using-oauth-2-0}

Salesforce使用OAuth通訊協定，讓應用程式的使用者能夠安全地存取（使用OAuth 2.0驗證應用程式）資料，而不需要揭露登入認證。 以下是將Marketo與Salesforce安全地連線和同步要執行的步驟。

>[!IMPORTANT]
>
>若要使用OAuth連線Marketo和Salesforce，請透過私人（無痕）瀏覽器登入Marketo，以避免使用錯誤的使用者名稱連線到Salesforce。

## 設定連線應用程式 {#set-up-connected-app}

1. 在Salesforce中的「設定」下，在「平台工具」中導覽至「應用程式」、「應用程式管理員」，然後按一下 **新連線應用程式**.

   ![](assets/setting-up-oauth-2-1.png)

1. 填寫詳細資料並按一下 **儲存**.

   ![](assets/setting-up-oauth-2-2.png)

1. 按一下 **啟用OAuth設定** 核取方塊。 對於回撥URL，請輸入 `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. 選取所有可用的OAuth範圍，然後按一下 **新增**.

   ![](assets/setting-up-oauth-2-3.png)

1. 按一下 **儲存**.

   ![](assets/setting-up-oauth-2-4.png)

1. 按一下 **繼續**.

   ![](assets/setting-up-oauth-2-5.png)

1. 複製使用者金鑰和使用者密碼。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>儲存消費者金鑰和使用者密碼資訊，以供日後在Marketo中使用。

## 設定Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必須為Salesforce Sync使用者啟用API存取（如果您是Salesforce Professional Edition使用者，預設情況下將無法使用該存取權 — 請聯絡您的Salesforce帳戶主管）。
>* 必須在Salesforce中建立Marketo Sync使用者。
>* 對於現有客戶，在客戶的訂閱上啟用「為SFDC同步啟用OAuth」功能。
>* 快顯封鎖程式已停用。
>* 已建立連線應用程式，且我們有消費者金鑰和消費者密碼可供使用。

>[!CAUTION]
>
>按一下之前，請務必先對同步使用者隱藏Marketo中所有不需要的欄位 **同步欄位**. 按一下「同步欄位」後，使用者可在SFDC中看見的所有欄位都會在Marketo中永久建立，且無法刪除。

1. 在「Marketo管理員」區段中，按一下 **CRM**，則 **與Salesforce同步**.

   ![](assets/setting-up-oauth-2-7.png)

1. 新增您先前錄製的消費者金鑰和消費者密碼資訊，然後按一下和 **儲存**.

   ![](assets/setting-up-oauth-2-8.png)

1. 在Marketo Salesforce同步頁面上，按一下 **使用Salesforce登入** 按鈕。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >如果您看到「使用者名稱/密碼/權杖」欄位而不是「使用Salesforce登入」按鈕，表示您的Marketo訂閱已啟用基本驗證。 請參閱 [使用基本驗證設定Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). 使用一組憑證開始同步後，Salesforce憑證或訂閱便不會切換。 如果您想要使用Oauth 2.0，請聯絡Adobe客戶團隊（您的客戶經理）。

1. 隨即顯示包含Salesforce登入頁面的快顯視窗。 輸入「Marketo同步使用者」認證並登入。

   ![](assets/setting-up-oauth-2-10.png)

1. 輸入您透過電子郵件（由Salesforce傳送）收到的驗證碼，然後按一下 **驗證**.

   ![](assets/setting-up-oauth-2-11.png)

1. 成功驗證後，存取頁面將顯示請求存取。 按一下 **允許**.

   ![](assets/setting-up-oauth-2-12.png)

1. 幾分鐘後，Marketo中會出現快顯視窗。 按一下 **確認認證**.

   ![](assets/setting-up-oauth-2-13.png)

1. 欄位同步完成後，請按一下 **開始Salesforce同步**.

   ![](assets/setting-up-oauth-2-14.png)

1. 按一下 **開始同步**.

   ![](assets/setting-up-oauth-2-15.png)

您目前正在Marketo和Salesforce之間同步。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [步驟1/3：將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [步驟2/3：建立Marketo (Enterprise/Unlimited)的Salesforce使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在SalesforceAppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
