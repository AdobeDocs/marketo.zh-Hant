---
unique-page-id: 11384018
description: 發行說明 — 16年秋季 — Marketo檔案 — 產品檔案
title: 發行說明 — 2016年秋季
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 發行說明：』16年秋季 {#release-notes-fall}

』16年秋季版包含下列功能。 查看您的Marketo版本以了解功能可用性。 請按一下標題連結，以檢視每項功能的詳細文章。

## 電子郵件中的預測內容 {#predictive-content-in-email}

我們的預測內容應用程式提供新的使用者體驗，可透過我們的機器學習和預測性演算法，在網路和電子郵件通道中追蹤、管理和建議您的內容。

>[!NOTE]
>
>在1月10日之前，所有具有預測模組的客戶都將啟用。

![](assets/shafe.png)

您現在可以將預測性內容新增至電子郵件。 開啟電子郵件時，收件者會自動收到相關的建議內容，以協助增加內容參與和轉換。

![](assets/predictive.png)

## [Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

透過Facebook離線轉換整合，Marketo中的轉換資料（針對銷售機會廣告銷售機會）會自動傳回至Facebook，讓您的廣告團隊能夠更妥善地最佳化其廣告支出。 在此Facebook Ad Manager報表中，會反白顯示離線轉換。

![](assets/facebook.png)

## [通用ID](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

通用ID可讓您透過單一登入存取多個Marketo訂閱，並快速在訂閱之間切換。 您可以對所有訂閱使用單一社群設定檔。

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>請聯絡Marketo支援以啟用此功能。

## Marketo帳戶型行銷增強功能 {#marketo-account-based-marketing-enhancements}

現在，您可以在「基於帳戶的行銷(ABM)」中將帳戶團隊指派給具名的帳戶，例如帳戶擁有者、銷售開發代表、業務開發代表和客戶成功經理。 您也可以建立帳戶擁有者專屬的帳戶清單，並將個人化的每週ABM報告傳送給帳戶團隊。

![](assets/account-team-11-15-16.png)

**REST API**

此版本也可讓您使用Marketo REST API在ABM中管理指名的帳戶屬性和帳戶分數。 如需API操作的詳細資訊，請造訪[Marketo開發人員網站](https://developers.marketo.com/rest-api/lead-database/named-accounts)。

## [稽核軌跡增強功能](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

稽核軌跡提供您在Marketo訂閱中所做變更的完整記錄。 我們已新增方案的其他追蹤功能，並呈現智慧型行銷活動、智慧清單以及使用者和角色所做變更的重要變更詳細資料。

## [新權限](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**讓電子郵件可運作**

讓使用者傳送交易式電子郵件給已取消訂閱之資料庫人員的擔心日子已經過去。 您現在可以指定哪些使用者可以讓電子郵件運作，或編輯操作電子郵件。

**編輯促銷活動限制**

如果您無法強制執行，為何要設定[促銷活動限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md)? 當您設定「促銷活動限制設定」以限制資料庫中可以以單一促銷活動定位的人數時，您現在可以限制哪些使用者可以在排程促銷活動時覆寫這些設定。

## [行動推播通知的音效](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

啟用音效，讓您的iOS推播通知更加豐富。 這項新功能可讓您在行動裝置上顯示推播通知時觸發音效。

>[!NOTE]
>
>* 裝置擁有者可以選擇在裝置設定中防止播放音效，而應用程式開發人員可在應用程式中提供裝置擁有者選項，以防止播放音效。
>* 推播通知在Android裝置上顯示時，會自動播放音效。


![](assets/sound-for-push-notifications.png)

## [與Salesforce加密相容的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight現在與Salesforce Shield Encryption相容。 所有Sales Insight客戶應升級到此最新的受管理軟體包（1.4359.2版），該軟體包[可在Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO)上獲得。

## [指定帳戶API](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

透過此版本，Marketo ABM使用者可透過指定帳戶API管理指定帳戶。 用戶可以建立、更新和刪除已命名的帳戶，以及讀取和更新ABM已命名的帳戶分數。

## [電子郵件編輯器v2.0 API支援](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

使用Marketo REST API管理v2.0格式的電子郵件變數和模組。

## [變更Marketo Salesforce同步](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

Marketo的Salesforce整合正在改善Marketo欄位與Salesforce同步的方式。 現在，您不必同步可能或可能不需要的大型欄位群組，而是可以挑選並選擇要包含的欄位。 如需詳細資訊，請前往這裡查看我們的檔案：[https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840)。
