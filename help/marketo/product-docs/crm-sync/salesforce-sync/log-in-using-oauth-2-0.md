---
description: 使用OAuth 2.0登錄 — Marketo文檔 — 產品文檔
title: 使用OAuth 2.0登錄
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
source-git-commit: c15753e0f2af199af8fd7e8bfe0924a915a39814
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 使用OAuth 2.0登錄 {#log-in-using-oauth-2-0}

Salesforce使用OAuth協定，允許應用程式用戶安全地訪問（使用OAuth 2.0驗證應用程式）資料，而不必洩露登錄憑據。 下面是要執行的步驟，以便安全地連接Marketo並與Salesforce同步。

>[!IMPORTANT]
>
>要使用OAuth連接Marketo和Salesforce，請通過私人（隱藏）瀏覽器登錄到Marketo，以避免使用錯誤的用戶名連接到Salesforce。

## 設定連接的應用 {#set-up-connected-app}

1. 在Salesforce中，在「設定」下，在「平台工具」中，導航到「應用」、「應用管理器」，然後按一下 **新連接的應用**。

   ![](assets/setting-up-oauth-2-1.png)

1. 填寫詳細資訊並按一下 **保存**。

   ![](assets/setting-up-oauth-2-2.png)

1. 按一下 **啟用OAuth設定** 複選框。 對於回叫URL，輸入 `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`。 選擇所有可用的OAuth作用域，然後按一下 **添加**。

   ![](assets/setting-up-oauth-2-3.png)

1. 按一下 **保存**。

   ![](assets/setting-up-oauth-2-4.png)

1. 按一下 **繼續**。

   ![](assets/setting-up-oauth-2-5.png)

1. 複製Consumer Key和Consumer Secret。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>保存消費者密鑰和消費者機密資訊，以供以後在Marketo使用。

## 設定Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必須為Salesforce Sync用戶啟用API訪問（如果您是Salesforce Professional Edition用戶，則預設情況下該訪問不可用 — 請與Salesforce帳戶主管聯繫）。
>* Marketo同步用戶必須在Salesforce中建立。
>* 對於現有客戶，在客戶的訂閱上啟用「為SFDC同步啟用OAuth」的功能。
>* 彈出窗口阻止程式已禁用。
>* 已建立已連接的應用，並且我們可以使用Consumer Key和Consumer Secret。


>[!CAUTION]
>
>在按一下之前，請確保在Marketo中隱藏您不需要的所有欄位 **同步欄位**。 按一下「同步欄位」後，用戶在SFDC中可以看到的所有欄位都將在Marketo永久建立，並且無法刪除。

1. 在「Marketo管理」部分，按一下 **CRM**，則 **與Salesforce同步**。

   ![](assets/setting-up-oauth-2-7.png)

1. 添加您以前記錄的Consumer Key和Consumer Secret資訊，然後按一下並 **保存**。

   ![](assets/setting-up-oauth-2-8.png)

1. 在MarketoSalesforce同步頁上，按一下 **使用Salesforce登錄** 按鈕

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >如果您看到的是「用戶名/密碼/令牌」欄位，而不是「使用Salesforce登錄」按鈕，則您的Marketo訂閱將啟用基本身份驗證。 請參閱 [設定具有基本身份驗證的Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)。 一旦同步開始使用一組憑據，則不會切換Salesforce憑據或訂閱。 如果要使用Oauth 2.0，請聯繫您的客戶成功經理。

1. 將顯示一個帶有salesforce登錄頁的彈出窗口。 「Marketo同步用戶」憑據中的密鑰並登錄。

   ![](assets/setting-up-oauth-2-10.png)

1. 輸入您通過電子郵件（由Salesforce發送）收到的驗證代碼，然後按一下 **驗證**。

   ![](assets/setting-up-oauth-2-11.png)

1. 成功驗證後，訪問頁面將顯示請求訪問。 按一下 **允許**。

   ![](assets/setting-up-oauth-2-12.png)

1. 幾分鐘後，一個彈出窗口將出現在Marketo。 按一下 **確認憑據**。

   ![](assets/setting-up-oauth-2-13.png)

1. 完成欄位同步後，按一下 **啟動Salesforce同步**。

   ![](assets/setting-up-oauth-2-14.png)

1. 按一下 **啟動同步**。

   ![](assets/setting-up-oauth-2-15.png)

您在Marketo和Salesforce之間的同步正在進行中。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [第1步（共3步）:將Marketo欄位添加到Salesforce（企業/無限制）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步（共3步）:為Marketo建立Salesforce用戶（企業/無限制）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在SalesforceAppExchange中安裝MarketoSales Insight軟體包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Enterprise/Unlimited中配置MarketoSales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

