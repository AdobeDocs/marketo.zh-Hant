---
unique-page-id: 11380218
description: 發行說明- 16年夏季-Marketo文檔——產品文檔
title: 發行說明- 16年夏季
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 發行說明：16年夏天{#release-notes-summer}

16年夏季版本包含下列功能。 查看您的Marketo版功能是否可用。 請按一下標題連結，以檢視每個功能的詳細文章。

## [帳戶型行銷](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo基於客戶的營銷在一個統一的平台中提供所有基本功能：

* **Target**  —— 帳戶發現、銷售線索到帳戶匹配和命名帳戶清單
* **參與** -帳戶型個人化、跨通道參與和帳戶專屬工作流程
* **衡量** -帳戶和清單層級的見解、帳戶參與分數，以及管道和收入影響

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM是您Marketo訂閱的附加元件，請連絡您的銷售代表以建置它。

## [稽核記錄](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

稽核記錄提供您在Marketo訂閱中所做變更的完整記錄。 它可讓使用者和管理員建立問責制，協助識別意外行為的原因，並提供安全性，讓您知道誰在做什麼和何時做什麼。 此資訊將可在任何時間點取得，並可用來回答下列問題：

* 此資產或設定發生了什麼情況，誰上次更新？
* X使用者最近做了什麼？
* 誰在登錄我們的帳戶？

![](assets/audit-trail.png)

## [Marketo-Vibes SMS LaunchPoint整合](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

直接在Marketo輕鬆建立簡訊。 使用您豐富的Marketo資料個人化並鎖定您的訊息，並使用SMS訊息儀表板輕鬆監控其效能。

>[!NOTE]
>
>此功能需要您有現有的Vibes SMS帳戶。

![](assets/vibes-sms2.png)

## [Email 2.0增強功能](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**模組層級變數**

以前，「電子郵件2.0範本」中指定的所有變數在範圍中都是「全域」。 在模組內使用變數時，如果您打算使用模組的多個例項，則不一定要這麼做。 在此版本中，變數現在可指定為「模組層級」，讓您指出使用者應該能夠針對其使用的每個模組設定唯一值。

![](assets/module-level-variables.png)

**語法更新**

* 您現在可以在「電子郵件2.0範本」中指定的模組上使用「mktoAddByDefault」，以指出新電子郵件中預設應顯示哪些模組。 如果您要建立包含大量模組的電子郵件範本，這會更方便。
* 在影像元素上，您現在可以指定是否應將底層`<img>` HTML元素的「height」和「width」屬性鎖定或編輯給使用者。 mktoLockImgSize=&quot;true&quot;會導致高度／寬度鎖定（即使影像已變更）。 同樣地，mktoLockImgStyle=&quot;true&quot;也會導致&quot;style&quot;屬性被鎖定。

**程式碼搜尋**

使用新的搜尋功能，以有效率地尋找並取代電子郵件程式碼中的內容。 此功能也可在「電子郵件範本」編輯器中使用。

![](assets/2nd-screenshot.png)

**影像元素中的Token支援**

Token現在可用於插入影像體驗的「外部URL」區域！ 如果您已使用`{{my.tokens}}`指定影像，現在可以在電子郵件編輯器2.0中參考這些Token。請注意，在「電子郵件編輯器2.0」畫布中，影像仍會顯示損毀。 但是，您會在傳送電子郵件之前，先在預覽和傳送範例中看到它們。

## 多個品牌網域{#multiple-branding-domains}

電子郵件追蹤連結只能以單一品牌網域加上品牌標示的日子已經一去不復返了。 您現在可以新增多個品牌網域，以激發消費者信心、建立更精簡的外觀以專注於品牌、改善電子郵件傳遞能力，並依每封電子郵件選擇要用於每個電子郵件追蹤連結的品牌網域。

![](assets/multiple-branding-domains.png)

## [方案Token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

我們為程式建立了新的Token類型。 您現在可以在資產和智慧型促銷活動流程步驟中演算方案名稱、說明和ID。

![](assets/program-tokens.png)

## [企業金鑰](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

要求銷售團隊中的每個人安裝我們的Sales Insight Plugin for Outlook可能很麻煩。 我們已引入新方式，使用企業金鑰遠端安裝Outlook增效模組。 將您在「管理員」的「Marketo銷售分析」區段中找到的獨特金鑰傳送給IT團隊，讓他們完成其餘工作。

![](assets/enterprise-key.png)

## [網頁個人化宣傳](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

指定網頁促銷活動在您網站上反應的延遲時間。

![](assets/dialog-campaign-delay.png)

## [內容分析與Recommendations匯出](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

離線檢視內容分析和建議資料。

## [電子郵件編輯器2.0的API支援](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

先前僅與v1.0電子郵件和範本相容的預先存在的資產API現在已針對v2.0電子郵件資產啟用。

## [Marketo開發商網站](https://developers.marketo.com/) {#marketo-developers-site}

全新改良！

## [隱私權設定](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

行銷人員可使用隱私權設定來決定是否使用Munchkin和Web個人化功能來追蹤訪客。 追蹤層級是使用瀏覽器的「不追蹤」設定、選擇退出Cookie或非特定IP來控制。 這些方法可能會影響Marketo在特定領域的價值和功能，但如果行銷人員未變更任何內容，Marketo的功能將維持不變。

此功能將在六週內逐步發佈給客戶。 如果您需要，請立即聯絡Marketo支援。
