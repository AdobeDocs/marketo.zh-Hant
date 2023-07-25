---
unique-page-id: 11380218
description: 發行說明 — 2016年夏季版 — Marketo檔案 — 產品檔案
title: 發行說明 — 2016年夏天
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 發行說明： 2016年夏天 {#release-notes-summer}

以下功能包含在2016年夏季發行版本中。 檢視您的Marketo版本，瞭解是否有功能可用。 請按一下標題連結以檢視每個功能的詳細文章。

## [以帳戶為基礎的行銷](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo帳戶式行銷在一個統一的平台上提供所有基本功能：

* **Target**  — 帳戶探索、銷售線索與帳戶的比對，以及具名帳戶清單
* **參與**  — 帳戶型個人化、跨管道參與和帳戶專屬工作流程
* **測量**  — 帳戶和清單層級的深入分析、帳戶參與度分數，以及管道和收入影響

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM可作為您Marketo訂閱的附加元件使用，請聯絡您的銷售代表以進行實施。

## [稽核軌跡](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

稽核軌跡提供您Marketo訂閱中所做變更的完整歷史記錄。 這樣可在使用者與管理員之間建立問責機制，有助於識別非預期行為的原因，並提供瞭解誰在做什麼以及何時做什麼的安全性。 此資訊可隨時取得，並可用於回答下列問題：

* 此資產或設定有什麼改變，上次更新的是誰？
* 使用者X最近做了什麼？
* 誰正在登入我們的帳戶？

![](assets/audit-trail.png)

## [Marketo-Vibes SMS LaunchPoint整合](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

直接在Marketo中輕鬆建立簡訊。 使用豐富的Marketo資料個人化和鎖定訊息，並使用SMS訊息儀表板輕鬆監控其效能。

>[!NOTE]
>
>此功能需要您擁有現有的Vibes SMS帳戶。

![](assets/vibes-sms2.png)

## [Email 2.0增強功能](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**模組層級變數**

先前，Email 2.0範本中指定的所有變數在範圍中都是「全域」。 在模組內使用變數時，如果您打算使用模組的多個例項，並不一定都希望如此。 在此版本中，變數現在可以指定為「模組層級」，這可讓您指示使用者應該能夠為其使用的每個模組設定唯一值。

![](assets/module-level-variables.png)

**語法更新**

* 您現在可以在電子郵件2.0範本中指定的模組上使用「mktoAddByDefault」，以指示預設應在新電子郵件中顯示哪些模組。 如果您要建立包含大量模組的電子郵件範本，這會方便得多。
* 在影像元素上，您現在可以指定基礎元素 `<img>` HTML元素的「高度」和「寬度」屬性應該鎖定或可供一般使用者編輯。 mktoLockImgSize=&quot;true&quot;會造成高度/寬度遭到鎖定（即使影像變更亦然）。 同樣地，mktoLockImgStyle=&quot;true&quot;會導致&quot;style&quot;屬性被鎖定。

**程式碼搜尋**

使用新的搜尋功能，有效率地尋找和取代電子郵件程式碼中的內容。 「電子郵件範本」編輯器中也提供此功能。

![](assets/2nd-screenshot.png)

**影像元素中的Token支援**

代號現在可用於插入影像體驗的「外部URL」區域！ 如果您已指定影像 `{{my.tokens}}`，您現在可以在電子郵件編輯器2.0中參考這些Token。請注意，在電子郵件編輯器2.0畫布中，影像仍會顯示為損毀。 但是，在傳送電子郵件之前，您會在預覽和傳送範例中看到它們呈現。

## 多個品牌領域 {#multiple-branding-domains}

電子郵件追蹤連結只能使用單一品牌網域來建立品牌的日子已經一去不復返了。 您現在可以新增多個品牌領域來激發消費者的信心、建立更精簡的外觀來著重於品牌、改善電子郵件傳遞能力，以及根據電子郵件選擇用於每個電子郵件追蹤連結的品牌領域。

![](assets/multiple-branding-domains.png)

## [計畫代號](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

我們已建立程式的新Token型別。 您現在可以在資產和智慧行銷活動流程步驟中轉譯方案名稱、說明和ID。

![](assets/program-tokens.png)

## [企業金鑰](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

要求您的銷售團隊中的每個人安裝適用於Outlook的Sales Insight外掛程式，可能會很枯燥。 我們匯入了使用企業金鑰從遠端安裝Outlook外掛程式的新方式。 將您在「管理員」的「Marketo銷售分析」區段中找到的唯一金鑰傳送給您的IT團隊，讓他們完成其餘工作。

![](assets/enterprise-key.png)

## [Web Personalization行銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

指定網站行銷活動在網站上反應的時間延遲。

![](assets/dialog-campaign-delay.png)

## [內容分析和Recommendations匯出](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

離線檢視內容分析和建議資料。

## [電子郵件編輯器2.0的API支援](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

先前僅與v1.0電子郵件和範本相容的既有資產API，現在可供v2.0電子郵件資產使用。

## [Marketo開發人員網站](https://developers.marketo.com/) {#marketo-developers-site}

全新及改良！

## [隱私權設定](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

行銷人員可使用隱私權設定，決定是否使用Munchkin和Web個人化功能追蹤訪客。 追蹤層級是使用瀏覽器的Do Not Track設定、選擇退出Cookie或非特定IP來控制。 這些方法可能會影響Marketo在特定領域的價值和功能，但如果行銷人員未變更任何專案，Marketo功能會維持不變。

此功能將在六週後逐步發行給客戶。 如果您需要立即取得此資訊，請聯絡Marketo支援。
