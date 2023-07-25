---
unique-page-id: 11384018
description: 發行說明–2016年秋季 — Marketo檔案 — 產品檔案
title: 發行說明 — 2016年秋季
exl-id: da935951-162e-426c-acf2-12c55ff706b4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 發行說明： 2016年秋季 {#release-notes-fall}

以下功能包含在2016年秋季版本中。 檢視您的Marketo版本，瞭解是否有功能可用。 請按一下標題連結以檢視每個功能的詳細文章。

## 電子郵件中的預測性內容 {#predictive-content-in-email}

我們的預測性內容應用程式有全新的使用者體驗，可透過我們的機器學習和預測性演演算法，在網路和電子郵件頻道追蹤、管理和建議您的內容。

>[!NOTE]
>
>1月10日前將啟用所有具有預測模組的客戶。

![](assets/shafe.png)

您現在可以將預測性內容新增至電子郵件。 開啟電子郵件時，收件者會自動收到相關、建議的內容，以協助提高內容參與度和轉換率。

![](assets/predictive.png)

## [facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

透過Facebook Offline Conversions整合，Marketo中的轉換資料（適用於潛在廣告銷售機會）會自動傳回Facebook，讓您的廣告團隊更能將其廣告支出最佳化。 在這份Facebook Ad Manager報表中，會強調離線轉換。

![](assets/facebook.png)

## [通用ID](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

通用ID可讓您透過單一登入存取多個Marketo訂閱，並快速在訂閱之間切換。 您可以對所有訂閱使用單一社群設定檔。

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>請聯絡Marketo支援以啟用此功能。

## Marketo帳戶型行銷增強功能 {#marketo-account-based-marketing-enhancements}

現在，您可以將帳戶團隊指派給帳戶型行銷(ABM)中的指定帳戶，例如，帳戶擁有者、銷售開發代表、業務開發代表和帳戶經理。 您也可以建立帳戶擁有者特定的帳戶清單，並將個人化的每週ABM報告傳送給帳戶團隊。

![](assets/account-team-11-15-16.png)

**REST API**

此版本也可讓您使用Marketo REST API在ABM中管理具名帳戶屬性和帳戶分數。 如需API操作的詳細資訊，請造訪 [Marketo開發人員網站](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [稽核軌跡增強功能](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

稽核軌跡提供您Marketo訂閱中所做變更的完整歷史記錄。 我們新增了方案的額外追蹤功能，並呈現智慧行銷活動的重要變更詳細資訊、智慧列示，以及對使用者和角色所做的變更。

## [新許可權](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md) {#new-permissions}

**讓電子郵件運作正常**

您必須擔心使用者傳送交易式電子郵件給資料庫中已取消訂閱之人員的日子已經過去。 您現在可以指定哪些使用者可以將電子郵件設為可操作，或編輯可操作的電子郵件。

**編輯行銷活動限制**

為何設定 [行銷活動限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) 如果您無法強制執行？ 當您設定「行銷活動限制設定」來限制資料庫中單一行銷活動可鎖定的人數，您現在便能夠在排程行銷活動時限制哪些使用者可以覆寫這些設定。

## [行動推播通知的聲音](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

啟用音效，讓您的iOS推播通知更加豐富。 這項新功能可讓您在行動裝置上顯示推播通知時觸發音效。

>[!NOTE]
>
>* 裝置擁有者可以選擇防止聲音在裝置設定中播放，應用程式開發人員則可在應用程式內為裝置擁有者提供選項，以防止聲音播放。
>* 在Android裝置上顯示推播通知時，會自動播放音效。

![](assets/sound-for-push-notifications.png)

## [Sales Insight與Salesforce Encryption相容](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight現在與Salesforce Shield Encryption相容。 所有Sales Insight客戶都應該升級至這個最新的Managed套件（1.4359.2版），也就是 [可在Appexchange上取得](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [具名帳戶API](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

透過此版本，Marketo ABM使用者可以透過指定帳戶API管理指定帳戶。 使用者可以建立、更新和刪除指定帳戶，以及讀取和更新ABM指定帳戶分數。

## [電子郵件編輯器v2.0 API支援](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

使用Marketo REST API管理v2.0格式的電子郵件變數和模組。

## [Marketo Salesforce同步處理的變更](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

Marketo的Salesforce整合不斷演化，以改善Marketo欄位與Salesforce同步的方式。 現在，您不必同步大量您可能需要（也可能不需要）的欄位，您可以挑選並選擇要包含的欄位。 如需詳細資訊，請在此處檢視我們的檔案： [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
