---
unique-page-id: 14352484
description: 如何修正連線至Salesforce時「我們無法驗證您的請求」 — Marketo檔案 — 產品檔案
title: 如何修正連接至 Salesforce 時發生的「我們無法驗證您的請求」問題
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 12%

---

# 如何修正連線到[!DNL Salesforce]時「我們無法驗證您的請求」 {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在嘗試將[!DNL Sales Connect]連線到[!DNL Salesforce]時收到錯誤訊息「我們無法驗證您的要求」，則您的存取[!DNL Salesforce]的API可能會受到限制。 請洽詢您的[!DNL Salesforce]管理員，確認下列專案已準備就緒。

## 在使用者許可權中啟用API {#enable-api-in-user-permissions}

1. 讓[!DNL Salesforce]管理員登入SFDC。
1. 選取「**[!UICONTROL Setup]**」。
1. 選取「**[!UICONTROL Manage Users]**」。
1. 選取「**[!UICONTROL Profiles]**」。
1. 尋找ToutApp使用者所在的設定檔，然後按一下&#x200B;**[!UICONTROL Edit]**。
1. 向下捲動至&#x200B;**[!UICONTROL Administrative Permissions]**，並確認已勾選&#x200B;**[!UICONTROL API Enabled]**。

## 檢查[!DNL Salesforce]是否正在封鎖[!DNL Sales Connect]的連線 {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 讓[!DNL Salesforce]管理員登入SFDC。
1. 選取「**[!UICONTROL Setup]**」。
1. 選取「**[!UICONTROL Manage Apps]**」。
1. 選取「**[!UICONTROL Connected Apps OAuth Usage]**」。
1. 請確定[!DNL Sales Connect]旁邊顯示「[!UICONTROL Block]」。 如果您看到&quot;[!UICONTROL Unblock]&quot;，請按一下按鈕以解除封鎖[!DNL Sales Connect]對[!DNL Salesforce]的存取權。
