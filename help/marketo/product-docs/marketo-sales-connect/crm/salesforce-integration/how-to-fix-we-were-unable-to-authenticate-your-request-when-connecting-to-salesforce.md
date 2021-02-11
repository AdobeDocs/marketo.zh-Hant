---
unique-page-id: 14352484
description: 如何修正連線至Salesforce —— 行銷人員檔案——產品檔案時的「我們無法驗證您的請求」
title: 如何修正連線至Salesforce時的「我們無法驗證您的請求」
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 如何修正連線至Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}時的「We Unable Unable Authenticate Your Request」

如果您在嘗試將Sales Connect連線至Salesforce時收到錯誤訊息「我們無法驗證您的請求」，則可能會限制您存取Salesforce的API。 請洽詢您的Salesforce管理員，以確定已有下列項目。

## 在使用者權限{#enable-api-in-user-permissions}中啟用API

1. 讓Salesforce管理員登入SFDC。
1. 選擇&#x200B;**Setup**。
1. 選擇&#x200B;**管理用戶**。
1. 選擇&#x200B;**配置檔案**。
1. 尋找ToutApp使用者所在的描述檔，然後按一下&#x200B;**編輯**。
1. 向下捲動至&#x200B;**管理權限**，並確定已勾選&#x200B;**啟用API**。

## 檢查Salesforce是否阻止Sales Connect從連接{#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 讓Salesforce管理員登入SFDC。
1. 選擇&#x200B;**Setup**。
1. 選擇&#x200B;**管理應用程式**。
1. 選擇「**連接的應用程式OAuth使用**」。
1. 請確定Sales Connect旁邊顯示「塊」。 如果您看到「取消阻止」，請按一下按鈕以取消阻止Sales Connect對Salesforce的訪問。
