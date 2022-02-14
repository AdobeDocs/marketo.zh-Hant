---
description: 登錄管理設定 — Marketo文檔 — 產品文檔
title: 登錄管理設定
hide: true
hidefromtoc: true
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
source-git-commit: 984a6dbd19d88db942d9d10bde4880a79feabcc7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 登錄管理設定 {#login-management-settings}

「登錄管理」設定允許管理員在全局級別為Sales Insight Actions的用戶設定身份驗證首選項。

>[!NOTE]
>
>預設情況下，將為Sales Insight Actions實例選擇Salesforce Only選項。 我們建議使用此設定，以便用戶 [自動登錄](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) 來自Salesforce。

## 更新登錄管理設定 {#update-login-management-settings}

>[!NOTE]
>
>**需要管理權限**

更新登錄管理首選項，請執行以下步驟。

1. 按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/login-management-settings-1.png)

1. 在「Admin Settings（管理設定）」下，按一下 **常規**。

   ![](assets/login-management-settings-2.png)

1. 向下滾動到登錄管理卡並選擇所需的設定（在本示例中，我們選擇的是僅Salesforce）。 按一下 **保存** 完成。

   ![](assets/login-management-settings-3.png)

## 僅限Salesforce常見問題 {#salesforce-only-faq}

僅Salesforce表示用戶只能通過身份驗證將Sales Insight Actions與Salesforce一起使用。 這是Sales Insight Actions實例的預設選擇，建議使用它是因為它允許用戶無縫地進行身份驗證而無需管理用戶名和密碼。

### 選擇「僅限Salesforce」時，我實例的新用戶如何激活其帳戶？ {#activate-when-salesforce-only-is-selected}

按一下 **入門** 按鈕，新用戶將被發送到帳戶激活螢幕，在該螢幕中，他們需要連接其Salesforce實例以激活其Sales Insight Actions帳戶。

![](assets/login-management-settings-4.png)

### 選擇「僅限Salesforce」時，我的用戶允許使用哪些身份驗證方法進行身份驗證？ {#what-authentication-methods}

導航到登錄螢幕時，用戶將首先輸入其電子郵件地址。 然後，他們將按一下Salesforce One Click Login按鈕，在此，他們可以使用登錄到的Salesforce帳戶進行身份驗證。

>[!NOTE]
>
>這僅適用於直接導航到登錄螢幕的用戶。 從Salesforce訪問Actions的用戶將登錄 [自動登錄](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md)。

![](assets/login-management-settings-5.png)

### 當用戶訪問Salesforce中的Actions功能並選擇「僅Salesforce」時，如何處理Actions的用戶身份驗證？ {#how-is-user-authentication-handled}

當用戶按一下其中一個操作（呼叫、電子郵件、市場活動、任務、市場活動清單等）時，我們會使用其SFDC身份驗證自動將其登錄到其Sales Insight Actions帳戶。 我們稱此身份驗證 [自動登錄](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md)。

## 所有登錄方法常見問題 {#all-login-methods-faq}

### 選擇「所有登錄方法」時，實例的新用戶如何激活其帳戶？ {#activate-when-all-login-methods-is-selected}

當新用戶被邀請訪問實例時，他們將收到帳戶激活電子郵件。 他們將按一下「開始」按鈕，然後將他們轉到要求他們建立並確認密碼的頁面。 建立後，將激活其帳戶，並通過登錄工作流將其接收。

![](assets/login-management-settings-6.png)

### 選擇「所有登錄方法」時，允許我實例的用戶使用什麼登錄？ {#what-are-users-allowed-to-log-in-with-all-login}

使用登錄頁時，用戶將首先輸入其電子郵件地址。 然後，它們將被發送到一個頁面，該頁面會為它們提供所有登錄選項（用戶名/密碼、 SFDC、Gmail、SSO），以進行身份驗證。
