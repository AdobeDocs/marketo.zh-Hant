---
description: 如何修正連線至Salesforce時「我們無法驗證您的請求」 — Marketo檔案 — 產品檔案
title: 如何在連線至Salesforce時修正「我們無法驗證您的請求」
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 如何在連線至Salesforce時修正「我們無法驗證您的請求」 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在嘗試將Sales Insight Actions連線至Salesforce時收到錯誤訊息「我們無法驗證您的請求」，表示您存取Salesforce的API可能會受到限制。 請洽詢您的Salesforce管理員，確認您已具備下列功能。

## 在使用者許可權中啟用API {#enable-api-in-user-permissions}

1. 讓Salesforce管理員登入SFDC。
1. 選取 **設定**.
1. 選取 **管理使用者**.
1. 選取 **設定檔**.
1. 尋找ToutApp使用者所在的設定檔，然後按一下 **編輯**.
1. 向下捲動至 **管理許可權** 並確定 **API已啟用** 已勾選。

## 檢查Salesforce是否封鎖銷售分析動作連線 {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. 請Salesforce管理員登入SFDC。
1. 選取 **設定**.
1. 選取 **管理應用程式**.
1. 選取 **連線應用程式OAuth使用方式**.
1. 請確定「銷售分析動作」旁邊顯示「封鎖」。 如果您看到「解除封鎖」，請按一下按鈕以解除封鎖Sales Insight Actions對Salesforce的存取權。
