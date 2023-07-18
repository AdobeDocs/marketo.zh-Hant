---
description: 設定Sales Insight Actions沙箱 — Marketo檔案 — 產品檔案
title: 設定Sales Insight動作沙箱
source-git-commit: 15c3124a53ce55810b598c43e29e21321534c81f
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 設定Sales Insight動作沙箱 {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions是以Web為基礎的應用程式，可透過 [Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. 有時稱為「Marketo銷售」，或簡稱為「動作」。

如果您有Marketo沙箱，您可以啟用動作例項來搭配沙箱用於測試目的。

設定Actions執行個體時，您必須決定將其設定為與Salesforce沙箱一起使用還是Salesforce生產搭配使用。 這是因為Salesforce對每個使用不同的端點，而Actions會使用與Salesforce的連線來啟動和驗證使用者。

請依照下列步驟操作，將Actions執行個體設定為與您的Salesforce沙箱執行個體搭配使用。

>[!NOTE]
>
>您可以進一步瞭解使用者將如何操作 [啟動其「動作」基座](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. You can also learn about how users will [authenticate with Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Additionally, if you prefer to have users authenticate with email and password, you can learn more about this in our [Login Management settings article](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## 要求將動作執行個體布建至您的Marketo沙箱 {#request=an-actions-instance}

除非有所要求，否則系統不會為Marketo沙箱執行個體啟用銷售分析動作。 聯絡Adobe客戶團隊（您的客戶經理）以提交請求。

## 為Marketo沙箱布建動作帳戶 {#provision-your-actions-account}

為您的Marketo沙箱啟用動作後，您將需要遵循以下步驟來啟用新的執行個體。

1. 登入您的Marketo沙箱執行個體。

1. 導覽至 **管理員**.

1. 選取 **銷售分析**.

1. 選取 **動作設定**.

   >[!IMPORTANT]
   >
   >電子郵件地址只能用於跨沙箱和生產執行個體的一個Actions執行個體。 如果您是管理員，且需要存取生產環境與沙箱中的多個執行個體，則必須針對每個執行個體使用不同的電子郵件地址。

1. 在布建卡中，選取您要邀請加入您的Sales Insight Actions執行個體的使用者。

## 啟動您的動作執行個體 {#activate-your-actions-instance}

您的Actions執行個體需要以Salesforce生產帳戶啟動。 啟動後，可切換至Salesforce Sandbox帳戶。

1. 找到已傳送的邀請。

1. 按一下 **開始使用** 連結。

1. 使用您的Salesforce生產執行個體啟動。

1. 按照提示來設定帳戶。 如需詳細概觀，請檢視我們的 [使用者入門文章](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## 準備您的Actions執行個體以與您的Salesforce沙箱執行個體相容 {#prepare-your-actions-instance}

動作需要您先使用Salesforce生產使用者啟動新執行個體。 啟動後，您可以使用以下步驟準備您的執行個體以與Salesforce沙箱相容。

1. 將登入設定更新為「所有登入方法」，以便您可以視需要使用使用者名稱和密碼登入。 若偏好使用，可在完成所有設定後，切換回「僅限Salesforce」。 [在這裡瞭解如何執行此操作](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. 中斷與Salesforce Production的連線，並連線至您的Salesforce沙箱。 [在此處瞭解如何連線](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. 對於步驟3，請選取「沙箱」而不是「Salesforce」。 如果您已經連線，應該會在Salesforce的「連線和自訂」標籤上看到中斷連線的選項。

>[!NOTE]
>
>如果您的Salesforce執行個體有自訂網域，建議在連線至Salesforce或登入Actions之前先登入您的Salesforce執行個體。

## 請求將您的Actions執行個體轉換為與您的Salesforce沙箱相容 {#request-your-actions-instance-be-converted}

1. 連絡人 [Marketo Engage支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} ，以要求將新的Sales Insight Actions執行個體設定為與Salesforce Sandbox相容。

1. 嘗試使用toutapp.com/login頁面上的「使用Salesforce登入」按鈕登入，以測試所有專案皆已正確設定。

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >如果您在此時發生任何問題，可以要求重設密碼，並使用密碼重新取得帳戶的存取權。

現在您的執行個體已準備好與您的Salesforce沙箱執行個體搭配使用。 如果您想要使用 [Salesforce自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} from Salesforce, you can switch back to "Salesforce Only" in your [Login Management settings](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [將您的Sales Insight Actions帳戶連結至Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Sales Insight Actions使用者入門指南](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [從Salesforce自動登入](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [登入管理設定](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
