---
description: 如何修正連線至Salesforce時「我們無法驗證您的請求」 — Marketo檔案 — 產品檔案
title: 如何在連線至Salesforce時修正「我們無法驗證您的請求」
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 如何在連線到[!DNL Salesforce]時修正「我們無法驗證您的請求」 {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您嘗試將Marketo Sales執行個體連線至Salesforce，但遇到「我們無法驗證您的請求」錯誤，此錯誤可能與Salesforce執行個體的設定有關。

有兩種型別的錯誤可能會產生此失敗的驗證頁面。

* 登入錯誤受限網域
* 已封鎖Oauth應用程式

您可以檢查URL以識別您要使用的型別。

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## 解決登入錯誤限制的網域 {#resolve-login-error-restricted-domain}

此錯誤通常表示您有一個無法路由到的自訂網域。 若要解決此錯誤，請嘗試先登入您要連線的Salesforce執行個體。 然後，請完成步驟以連線至Salesforce。

如果您嘗試連線的執行個體是Salesforce沙箱網域，而您收到錯誤，您將需要執行其他步驟，將執行個體更新為相容於Salesforce沙箱。 [了解更多](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}。

## 解決Oauth應用程式遭到封鎖的問題 {#resolve-oauth-app-blocked}

如果您在URL中收到錯誤訊息「我們無法驗證您的請求」，且含有Oauth應用程式封鎖的錯誤型別（或其他型別），表示您存取Salesforce的API可能會受到限制。 請洽詢您的Salesforce管理員，確認下列專案已準備就緒。

### 在使用者許可權中啟用API {#enable-api-in-user-permissions}

1. 請Salesforce管理員登入Salesforce。
1. 選取&#x200B;**安裝程式**。
1. 選取&#x200B;**管理使用者**。
1. 選取&#x200B;**設定檔**。
1. 尋找ToutApp使用者所在的設定檔，然後按一下&#x200B;**編輯**。
1. 向下捲動至&#x200B;**系統管理許可權**，並確認已勾選&#x200B;**已啟用API**。

### 檢查Salesforce是否封鎖銷售Insight動作連線 {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. 請Salesforce管理員登入Salesforce。
1. 選取&#x200B;**安裝程式**。
1. 選取&#x200B;**管理應用程式**。
1. 選取&#x200B;**連線應用程式OAuth使用方式**。
1. 請確定銷售Insight動作旁邊顯示「封鎖」。 如果您看到「解除封鎖」，請按一下按鈕，以解除封鎖銷售Insight動作對Salesforce的存取。
