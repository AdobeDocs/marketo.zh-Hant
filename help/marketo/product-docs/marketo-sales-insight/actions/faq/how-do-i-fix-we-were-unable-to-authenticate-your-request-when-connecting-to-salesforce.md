---
description: 連線至Salesforce - Marketo檔案 — 產品檔案時，如何修正「我們無法驗證您的請求」
title: 如何修正連接到Salesforce時「我們無法驗證您的請求」
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 如何修正連接到Salesforce時「我們無法驗證您的請求」 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在嘗試將Sales Insight Actions連結至Salesforce時收到「We un aunable to authenticate your request」錯誤訊息，則您對Salesforce的API的存取權可能會受到限制。 請洽詢您的Salesforce管理員，確認有下列項目。

## 在使用者權限中啟用API {#enable-api-in-user-permissions}

1. 讓Salesforce管理員登錄到SFDC。
1. 選擇 **設定**.
1. 選擇 **管理使用者**.
1. 選擇 **設定檔**.
1. 查找ToutApp用戶所在的配置檔案，然後按一下 **編輯**.
1. 向下捲動至 **管理權限** 確保 **啟用API** 已勾選。

## 檢查Salesforce是否阻止Sales Insight操作連接 {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. 讓Salesforce管理員登錄到SFDC。
1. 選擇 **設定**.
1. 選擇 **管理應用程式**.
1. 選擇 **連線應用程式OAuth使用狀況**.
1. 請確定「銷售分析動作」旁顯示「區塊」。 如果您看到「解除封鎖」，請按一下按鈕以解除封鎖Salesforce的Sales Insight Actions存取權。
