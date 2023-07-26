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

登入管理設定可讓管理員為全域層級的Sales Insight Actions使用者設定驗證偏好設定。

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

1. 在管理設定下，按一下 **一般**.

   ![](assets/login-management-settings-2.png)

1. 向下捲動至「登入管理」卡片，並選取所需的設定（在此範例中，我們選擇「僅限Salesforce」）。 按一下 **儲存** 完成時。

   ![](assets/login-management-settings-3.png)

## 僅限Salesforce常見問題集 {#salesforce-only-faq}

「僅限Salesforce」表示使用者只能驗證是否透過Salesforce使用Sales Insight Actions。 這是Sales Insight Actions執行個體的預設選項，之所以推薦使用，是因為它可讓使用者無縫驗證，而不需要管理使用者名稱和密碼。

### 當選取「僅限Salesforce」時，我執行個體的新使用者如何啟動其帳戶？ {#activate-when-salesforce-only-is-selected}

按一下 **快速入門** 邀請電子郵件中的按鈕，新使用者將被傳送至帳戶啟動畫面，要求他們連線Salesforce執行個體以啟動其Sales Insight Actions帳戶。

![](assets/login-management-settings-4.png)

### 選擇「僅限Salesforce」時，允許我的使用者使用哪些驗證方法進行驗證？ {#what-authentication-methods}

導覽至我們的登入畫面時，使用者會先輸入電子郵件地址。 接著，他們會按一下Salesforce一鍵登入按鈕，在那裡他們可以使用他們登入的Salesforce帳戶進行驗證。

>[!NOTE]
>
>這僅與直接導覽至登入畫面的使用者有關。 從Salesforce存取動作的使用者將會登入 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### 當使用者從Salesforce存取動作功能並選取「僅限Salesforce」時，如何處理動作的使用者驗證？ {#how-is-user-authentication-handled}

當使用者按一下其中一個動作（通話、電子郵件、行銷活動、任務、行銷活動清單等……）時，我們會使用他們的SFDC驗證來自動將其登入他們的銷售分析動作帳戶。 我們稱之為「驗證」 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## 所有登入方法常見問題集 {#all-login-methods-faq}

### 選取「所有登入方法」時，我執行個體的新使用者如何啟動其帳戶？ {#activate-when-all-login-methods-is-selected}

當新的使用者受邀加入執行個體時，他們將收到帳戶啟用電子郵件。 他們將會按一下顯示「開始使用」的按鈕，然後前往要求他們建立並確認密碼的頁面。 建立後，他們的帳戶將會啟用，並透過上線工作流程領取。

![](assets/login-management-settings-6.png)

### 選取「所有登入方法」時，允許我執行個體的使用者使用哪些登入？ {#what-are-users-allowed-to-log-in-with-all-login}

使用我們的登入頁面時，使用者將先輸入其電子郵件地址。 接著，系統會將他們傳送至一個頁面，提供他們所有登入選項（使用者名稱/密碼、SFDC、Gmail、SSO），以使用進行驗證。
