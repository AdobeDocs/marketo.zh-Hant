---
description: 登入管理設定 — Marketo檔案 — 產品檔案
title: 登入管理設定
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 登入管理設定 {#login-management-settings}

「登入管理」設定可讓管理員為全域層級的「銷售分析動作」使用者設定驗證偏好設定。

>[!NOTE]
>
>預設情況下，將為「銷售分析操作」實例選擇「僅限Salesforce」選項。 建議您使用此設定，讓使用者能夠 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) 來自Salesforce。

## 更新登入管理設定 {#update-login-management-settings}

>[!NOTE]
>
>**需要管理員權限**

請依照下列步驟更新登入管理偏好設定。

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/login-management-settings-1.png)

1. 在「管理設定」下，按一下 **一般**.

   ![](assets/login-management-settings-2.png)

1. 向下捲動至「登入管理」卡，然後選取所需的設定（在此範例中，我們選擇「僅限Salesforce」）。 按一下 **儲存** 時才能使用。

   ![](assets/login-management-settings-3.png)

## 僅限Salesforce常見問題集 {#salesforce-only-faq}

僅限Salesforce表示用戶只能通過驗證來使用Salesforce的Sales Insight Actions。 這是Sales Insight Actions實例的預設選擇，建議使用它，因為它允許用戶無縫地進行身份驗證，而不需要管理用戶名和密碼。

### 選取「僅限Salesforce」時，我執行個體的新使用者如何啟用其帳戶？ {#activate-when-salesforce-only-is-selected}

按一下 **快速入門** 按鈕，新使用者將會被傳送至帳戶啟用畫面，在畫面中，新使用者將需要連接其Salesforce執行個體以啟用其Sales Insight Actions帳戶。

![](assets/login-management-settings-4.png)

### 選取「僅限Salesforce」時，我的使用者可以透過哪些驗證方法進行驗證？ {#what-authentication-methods}

導覽至登入畫面時，使用者會先輸入其電子郵件地址。 然後，他們將按一下「Salesforce一鍵登錄」按鈕，在該按鈕中，他們可以使用登錄到的Salesforce帳戶進行身份驗證。

>[!NOTE]
>
>這隻與直接導覽至登入畫面的使用者有關。 從Salesforce存取「動作」的使用者將以 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### 當用戶從Salesforce中訪問「操作」功能，並選擇「僅限Salesforce」時，如何為「操作」處理用戶身份驗證？ {#how-is-user-authentication-handled}

當用戶按一下其中一個操作（呼叫、電子郵件、促銷活動、任務、促銷活動清單等）時，我們會使用其SFDC驗證自動將其登錄到其Sales Insight Actions帳戶。 我們稱此驗證為 [自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## 所有登入方法常見問題集 {#all-login-methods-faq}

### 選取「所有登入方法」時，我例項的新使用者會如何啟用其帳戶？ {#activate-when-all-login-methods-is-selected}

當新使用者受邀加入執行個體時，他們會收到帳戶啟用電子郵件。 他們將按一下顯示「開始使用」的按鈕，接著頁面會要求他們建立並確認密碼。 建立帳戶後，其帳戶就會啟動，並透過入門工作流程執行。

![](assets/login-management-settings-6.png)

### 選取「所有登入方法」時，我例項的使用者可以透過哪些項目登入？ {#what-are-users-allowed-to-log-in-with-all-login}

使用登入頁面時，使用者會先輸入其電子郵件地址。 然後，這些檔案會傳送至頁面，提供所有登入選項（使用者名稱/密碼、SFDC、Gmail、SSO），供其驗證。
