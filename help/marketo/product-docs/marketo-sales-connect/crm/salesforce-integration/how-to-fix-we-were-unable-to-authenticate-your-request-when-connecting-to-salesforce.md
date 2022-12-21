---
unique-page-id: 14352484
description: 如何修正連線至Salesforce - Marketo檔案 — 產品檔案時的「We Unable Unable To Authenticate Your Request」
title: 如何修正連線至Salesforce時的「We Unable Unable To Authenticate Your Request」
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 如何修正連線至Salesforce時的「We Unable Unable To Authenticate Your Request」 {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在嘗試將Sales Connect連接到Salesforce時收到「We unable to authenticate your request」錯誤消息，則您對Salesforce的API的訪問可能會受到限制。 請洽詢您的Salesforce管理員，確認有下列項目。

## 在使用者權限中啟用API {#enable-api-in-user-permissions}

1. 讓Salesforce管理員登錄到SFDC。
1. 選擇 **設定**.
1. 選擇 **管理使用者**.
1. 選擇 **設定檔**.
1. 查找ToutApp用戶所在的配置檔案，然後按一下 **編輯**.
1. 向下捲動至 **管理權限** 確保 **啟用API** 已勾選。

## 檢查Salesforce是否阻止Sales Connect連接 {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 讓Salesforce管理員登錄到SFDC。
1. 選擇 **設定**.
1. 選擇 **管理應用程式**.
1. 選擇 **連線應用程式OAuth使用狀況**.
1. 確保Sales Connect旁邊顯示「Block」。 如果看到「解除阻止」，請按一下按鈕以解除阻止Sales Connect對Salesforce的訪問。
