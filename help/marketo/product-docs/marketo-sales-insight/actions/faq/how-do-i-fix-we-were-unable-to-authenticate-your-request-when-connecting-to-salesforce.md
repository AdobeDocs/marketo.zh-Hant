---
description: 連接到Salesforce -Marketo文檔 — 產品文檔時，如何修復「We We Unable to Authenticate Your Request」
title: 連接到Salesforce時如何修復「我們無法驗證您的請求」
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 連接到Salesforce時如何修復「我們無法驗證您的請求」 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在嘗試將Sales Insight Actions連接到Salesforce時收到錯誤消息「We wae we cannot authenticate your request」，則可能會限制您對Salesforce API的訪問。 請咨詢您的Salesforce管理員，確保已部署以下內容。

## 在用戶權限中啟用API {#enable-api-in-user-permissions}

1. 讓Salesforce管理員登錄到SFDC。
1. 選擇 **設定**。
1. 選擇 **管理用戶**。
1. 選擇 **配置檔案**。
1. 查找ToutApp用戶所在的配置檔案，然後按一下 **編輯**。
1. 向下滾動到 **管理權限** 確保 **已啟用API** 的子菜單。

## 檢查Salesforce是否阻止Sales Insight活動連接 {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. 讓Salesforce Admin登錄到SFDC。
1. 選擇 **設定**。
1. 選擇 **管理應用**。
1. 選擇 **已連接的應用OAuth用法**。
1. 確保Sales Insight Actions旁邊顯示「Block」。 如果看到「取消阻止」，請按一下按鈕以取消阻止Sales Insight Actions對Salesforce的訪問。
