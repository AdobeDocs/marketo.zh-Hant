---
description: 設定OAuth 2.0 -Marketo檔案——產品檔案
title: 設定OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 設定OAuth 2.0 {#setting-up-oauth-2-0}

Salesforce使用OAuth通訊協定，讓應用程式的使用者透過REST API呼叫安全地存取（使用OAuth 2.0驗證應用程式）資料，而不需揭露登入憑證。 以下是要執行的步驟，以安全地連接Marketo與Salesforce並同步化。

## 設定連線的應用程式{#set-up-connected-app}

1. 在Salesforce的「設定」下，在「平台工具」中，導覽至「應用程式」、「應用程式管理員」，然後按一下「新連線的應用程式」**。**

   ![](assets/setting-up-oauth-2-1.png)

1. 填寫詳細資訊，然後按一下「儲存」。****

   ![](assets/setting-up-oauth-2-2.png)

1. 按一下「啟用OAuth設定&#x200B;**」核取方塊。**&#x200B;在回呼URL中，輸入`https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`。 選擇所有可用的OAuth示波器，然後按一下&#x200B;**添加**。

   ![](assets/setting-up-oauth-2-3.png)

1. 按一下&#x200B;**保存**。

   ![](assets/setting-up-oauth-2-4.png)

1. 按一下&#x200B;**繼續**。

   ![](assets/setting-up-oauth-2-5.png)

1. 複製消費者金鑰和消費者機密。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>儲存消費者金鑰和消費者機密資訊，以供日後在Marketo使用。

## 設定Marketo{#set-up-marketo}

>[!PREREQUISITES]
>
>* 必須為Salesforce Sync使用者啟用API存取權（如果您是Salesforce Professional Edition使用者，該存取權預設不可用——請連絡您的Salesforce帳戶主管）。
>* Marketo同步使用者必須在Salesforce中建立。
>* 對於現有客戶，客戶的訂閱中啟用「啟用OAuth for SFDC同步」功能。
>* 快顯封鎖程式已停用。
>* 已建立連線的應用程式，我們提供消費者金鑰和消費者密碼供使用。


1. 在「Marketo管理員」區段中，按一下&#x200B;**CRM**，然後按一下&#x200B;**與Salesforce**&#x200B;同步。

   ![](assets/setting-up-oauth-2-7.png)

1. 新增您先前記錄的使用者金鑰和使用者密碼資訊，然後按一下並&#x200B;**儲存**。

   ![](assets/setting-up-oauth-2-8.png)

1. 在「MarketoSalesforce同步」頁面上，按一下「使用Salesforce登入&#x200B;**」按鈕。**

   ![](assets/setting-up-oauth-2-9.png)

1. 將會顯示包含salesforce登入頁面的快顯視窗。 您的「Marketo同步用戶」憑證中的密鑰並登錄。

   ![](assets/setting-up-oauth-2-10.png)

1. 輸入您透過電子郵件（由Salesforce傳送）收到的驗證碼，然後按一下「驗證」。****

   ![](assets/setting-up-oauth-2-11.png)

1. 成功驗證後，存取頁面會顯示要求存取。 按一下&#x200B;**允許**。

   ![](assets/setting-up-oauth-2-12.png)

1. 幾分鐘後，Marketo將出現快顯視窗。 按一下&#x200B;**確認憑據**。

   ![](assets/setting-up-oauth-2-13.png)

1. 完成欄位同步後，按一下「啟動Salesforce同步」。****

   ![](assets/setting-up-oauth-2-14.png)

1. 按一下&#x200B;**開始同步**。

   ![](assets/setting-up-oauth-2-15.png)

您在Marketo和Salesforce之間的同步現在正在進行中。

![](assets/setting-up-oauth-2-16.png)
