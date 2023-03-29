---
description: 使用OAuth 2.0登入 — Marketo檔案 — 產品檔案
title: 使用OAuth 2.0登入
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 使用OAuth 2.0登入 {#log-in-using-oauth-2-0}

Salesforce使用OAuth通訊協定，讓應用程式的使用者不必透露登入憑證，就能安全地存取（使用OAuth 2.0驗證應用程式）資料。 以下是要執行的步驟，以便安全地連接Marketo並與Salesforce同步。

>[!IMPORTANT]
>
>若要使用OAuth連線Marketo和Salesforce，請透過私人（無痕）瀏覽器登入Marketo，以免使用錯誤的使用者名稱連線至Salesforce。

## 設定連線的應用程式 {#set-up-connected-app}

1. 在Salesforce中，在「設定」下，在「平台工具」中，導覽至「應用程式」、「應用程式管理員」，然後按一下 **新連線應用程式**.

   ![](assets/setting-up-oauth-2-1.png)

1. 填寫詳細資訊，然後按一下 **儲存**.

   ![](assets/setting-up-oauth-2-2.png)

1. 按一下 **啟用OAuth設定** 核取方塊。 對於回呼URL，請輸入 `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. 選擇所有可用的OAuth作用域，然後按一下 **新增**.

   ![](assets/setting-up-oauth-2-3.png)

1. 按一下 **儲存**.

   ![](assets/setting-up-oauth-2-4.png)

1. 按一下 **繼續**.

   ![](assets/setting-up-oauth-2-5.png)

1. 複製使用者金鑰和使用者密碼。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>儲存使用者金鑰和使用者密碼資訊，以供稍後在Marketo中使用。

## 設定Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必須為Salesforce同步用戶啟用API訪問（如果您是Salesforce Professional Edition用戶，預設情況下該訪問不可用 — 請與您的Salesforce帳戶主管聯繫）。
>* Marketo同步使用者必須在Salesforce中建立。
>* 針對現有客戶，在客戶訂閱上啟用「為SFDC同步啟用OAuth」功能。
>* 快顯視窗封鎖程式會停用。
>* 已建立連線應用程式，且使用者金鑰和使用者密碼可供使用。


>[!CAUTION]
>
>請務必隱藏Marketo中不需要的所有欄位，不要讓同步使用者按一下 **同步欄位**. 按一下「同步欄位」後，用戶在SFDC中看到的所有欄位都將在Marketo中永久建立，並且無法刪除。

1. 在「Marketo管理員」區段中，按一下 **CRM**，然後 **與Salesforce同步**.

   ![](assets/setting-up-oauth-2-7.png)

1. 新增您先前記錄的使用者金鑰和使用者密碼資訊，然後按一下並 **儲存**.

   ![](assets/setting-up-oauth-2-8.png)

1. 在Marketo Salesforce同步頁面上，按一下 **使用Salesforce登入** 按鈕。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >如果您看到的是「使用者名稱/密碼/代號」欄位，而不是「使用Salesforce登入」按鈕，表示您的Marketo訂閱已啟用基本驗證。 請參閱 [使用基本驗證設定Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). 一旦使用一組憑據開始同步，Salesforce憑據或訂閱便不會切換。 如果您想使用Oauth 2.0，請洽詢Adobe帳戶團隊（您的帳戶管理員）。

1. 將顯示帶有salesforce登入頁面的快顯視窗。 「Marketo同步使用者」憑證中的金鑰並登入。

   ![](assets/setting-up-oauth-2-10.png)

1. 輸入您通過電子郵件（由Salesforce發送）收到的驗證代碼，然後按一下 **驗證**.

   ![](assets/setting-up-oauth-2-11.png)

1. 成功驗證後，存取頁面會顯示請求存取。 按一下 **允許**.

   ![](assets/setting-up-oauth-2-12.png)

1. 幾分鐘後，快顯視窗會出現在Marketo。 按一下 **確認憑證**.

   ![](assets/setting-up-oauth-2-13.png)

1. 欄位同步完成後，按一下 **啟動Salesforce同步**.

   ![](assets/setting-up-oauth-2-14.png)

1. 按一下 **開始同步**.

   ![](assets/setting-up-oauth-2-15.png)

您在Marketo和Salesforce之間的同步現在正在進行中。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [第1步（共3步）:將Marketo欄位新增至Salesforce（企業版/無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步（共3步）:建立Marketo的Salesforce使用者（企業版/無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在SalesforceAppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

