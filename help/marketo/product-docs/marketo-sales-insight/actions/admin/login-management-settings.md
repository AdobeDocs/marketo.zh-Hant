---
description: 登入管理設定 — Marketo檔案 — 產品檔案
title: 登入管理設定
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 登入管理設定 {#login-management-settings}

登入管理設定可讓管理員在全域層級設定Sales Insight Actions使用者的驗證偏好設定。

>[!NOTE]
>
>依預設，系統將會針對「銷售分析動作」執行個體選取「僅限Salesforce」選項。 我們建議使用此設定，讓使用者可以 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) 來自Salesforce。

## 更新登入管理設定 {#update-login-management-settings}

>[!NOTE]
>
>**需要管理員許可權**

請依照以下步驟更新您的登入管理偏好設定。

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/login-management-settings-1.png)

1. 在「管理設定」底下，按一下 **一般**.

   ![](assets/login-management-settings-2.png)

1. 向下捲動至「登入管理」卡片並選取所需的設定（在此範例中，我們選擇「僅限Salesforce」）。 按一下 **儲存** 完成時。

   ![](assets/login-management-settings-3.png)

## 僅限Salesforce常見問題集 {#salesforce-only-faq}

Salesforce Only表示使用者只能驗證以搭配Salesforce使用Sales Insight Actions。 這是Sales Insight Actions執行個體的預設選擇，之所以推薦使用，是因為它允許使用者無縫驗證，而不需要管理使用者名稱和密碼。

### 當選取「僅限Salesforce」時，我執行個體的新使用者如何啟動其帳戶？ {#activate-when-salesforce-only-is-selected}

按一下 **快速入門** 按鈕時，系統會將新使用者傳送至帳戶啟動畫面，要求他們連線其Salesforce執行個體以啟動其Sales Insight Actions帳戶。

![](assets/login-management-settings-4.png)

### 選擇「僅限Salesforce」時，允許我的使用者使用哪些驗證方法進行驗證？ {#what-authentication-methods}

導覽至我們的登入畫面時，使用者會先輸入其電子郵件地址。 接著，訪客會按一下Salesforce一鍵登入按鈕，接著可以使用登入的Salesforce帳戶進行驗證。

>[!NOTE]
>
>這僅適用於直接導覽至登入畫面的使用者。 從Salesforce存取Actions的使用者將以下列身分登入 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### 當使用者從Salesforce存取動作功能並選取「僅限Salesforce」時，如何處理動作的使用者驗證？ {#how-is-user-authentication-handled}

當使用者按一下其中一個動作（通話、電子郵件、行銷活動、任務、行銷活動清單等……）時，我們會使用他們的SFDC驗證來自動將其登入他們的銷售分析動作帳戶。 我們稱之為此驗證 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## 所有登入方法常見問題集 {#all-login-methods-faq}

### 選取「所有登入方法」時，我執行個體的新使用者如何啟用其帳戶？ {#activate-when-all-login-methods-is-selected}

當新使用者受邀加入執行個體時，他們將收到帳戶啟用電子郵件。 他們將會按一下顯示「開始」的按鈕，然後帶他們到一個要求他們建立和確認密碼的頁面。 建立此專案後，其帳戶將會啟用，並透過上線工作流程引導他們。

![](assets/login-management-settings-6.png)

### 選取「所有登入方法」時，我的執行個體的使用者可以使用哪些登入？ {#what-are-users-allowed-to-log-in-with-all-login}

使用我們的登入頁面時，使用者將先輸入其電子郵件地址。 接著，系統會將使用者傳送至一個頁面，該頁面會提供使用者所有登入選項（使用者名稱/密碼、SFDC、Gmail、SSO），以便使用者進行驗證。
