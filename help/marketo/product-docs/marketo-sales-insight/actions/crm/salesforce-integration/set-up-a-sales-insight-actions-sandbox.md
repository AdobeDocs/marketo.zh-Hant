---
description: 設定銷售Insight動作沙箱 — Marketo檔案 — 產品檔案
title: 設定銷售洞察動作沙箱
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 2%

---

# 設定銷售洞察動作沙箱 {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions是網頁式應用程式，透過[Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}專門與Salesforce CRM整合。 有時稱為「Marketo銷售」，或簡稱為「動作」。

如果您有Marketo沙箱，您可以啟用動作執行個體來搭配沙箱用於測試目的。

設定Actions執行個體時，您必須決定其將設定為搭配Salesforce Sandbox或Salesforce生產使用。 這是因為Salesforce對每個使用不同的端點，而動作會使用與Salesforce的連線來啟動和驗證使用者。

請依照下列步驟，將Actions執行個體設定為與您的Salesforce沙箱執行個體搭配使用。

>[!NOTE]
>
>您可以進一步瞭解使用者如何[啟動其「動作」座位](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}。 您也可以瞭解使用者將如何[使用Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}進行驗證。 此外，如果您偏好讓使用者使用電子郵件和密碼進行驗證，您可在[「登入管理」設定文章](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}中進一步瞭解此資訊。

## 要求將動作執行個體布建至您的Marketo沙箱 {#request=an-actions-instance}

除非有所要求，否則系統不會為Marketo沙箱例項啟用銷售Insight動作。 聯絡Adobe客戶團隊（您的客戶經理）以提交請求。

## 針對Marketo沙箱布建您的動作帳戶 {#provision-your-actions-account}

在為Marketo沙箱啟用動作後，您需要依照下列步驟啟用新執行個體。

1. 登入您的Marketo沙箱執行個體。

1. 瀏覽至&#x200B;**管理員**。

1. 選取&#x200B;**銷售Insight**。

1. 選取&#x200B;**動作設定**。

   >[!IMPORTANT]
   >
   >電子郵件地址只能用於沙箱和生產執行個體中的一個動作執行個體。 如果您是管理員，且需要存取生產環境與沙箱中的多個執行個體，則必須針對每個執行個體使用不同的電子郵件地址。

1. 在布建卡中，選取您要邀請加入銷售Insight動作執行個體的使用者。

## 啟動您的動作執行個體 {#activate-your-actions-instance}

您的Actions執行個體需要使用Salesforce生產帳戶啟用。 啟用後，可將其切換至Salesforce沙箱帳戶。

1. 找出已傳送的邀請。

1. 按一下&#x200B;**開始使用**&#x200B;連結。

1. 使用您的Salesforce生產執行個體啟用。

1. 按照提示來設定帳戶。 如需詳細概觀，請參閱我們的[使用者入門文章](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}。

## 準備您的Actions執行個體以與您的Salesforce沙箱執行個體相容 {#prepare-your-actions-instance}

動作需要您先透過Salesforce生產使用者啟用新執行個體。 啟動後，您可以使用以下步驟準備您的執行個體以與Salesforce沙箱相容。

1. 將登入設定更新為「所有登入方法」，以便您可以視需要使用使用者名稱和密碼登入。 如果偏好設定，可在完成所有設定後切換回「僅限Salesforce」。 [在此檢視如何執行此動作](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}。

1. 中斷與Salesforce生產環境的連線，並連線至您的Salesforce沙箱。 [瞭解如何在這裡連線](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}。 在步驟3中，選取「沙箱」而非「Salesforce」。 如果您已經連線，您應該會在Salesforce的「連線和自訂」標籤上看到中斷連線的選項。

>[!NOTE]
>
>如果您的Salesforce執行個體有自訂網域，建議先登入您的Salesforce執行個體，再連線至Salesforce或登入「動作」。

## 請求將您的Actions執行個體轉換為與您的Salesforce沙箱相容 {#request-your-actions-instance-be-converted}

1. 請連絡[Marketo Engage支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}，要求將您新的Sales Insight Actions執行個體設定為與Salesforce Sandbox相容。

1. 嘗試使用toutapp.com/login頁面上的「使用Salesforce登入」按鈕登入，以測試所有專案皆已正確設定。

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >如果您在此遇到任何問題，可以要求重設密碼，並使用密碼重新取得帳戶的存取權。

現在，您的執行個體已準備好與您的Salesforce沙箱執行個體搭配使用。 如果您想從Salesforce使用[Salesforce自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}，可以在[登入管理設定](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}中切換回「僅限Salesforce」。

>[!NOTE]
>
>* [將您的Sales Insight Actions帳戶連線至Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [銷售Insight動作使用者入門指南](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [從Salesforce自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [登入管理設定](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
