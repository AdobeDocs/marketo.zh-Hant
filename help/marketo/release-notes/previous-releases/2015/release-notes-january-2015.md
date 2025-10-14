---
unique-page-id: 4720758
description: 發行說明 — 2015年1月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2015年1月
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 1%

---

# 發行說明：2015 年 1 月 {#release-notes-january}

2015年1月發行版本包含下列功能。 請檢查您的Marketo版本是否有功能可用。 發行後，請務必返回尋找每個功能的詳細文章連結！

## 行銷自動化更新 {#marketing-automation-updates}

**支援行動裝置的登陸頁面**

您現在可以從登入頁面編輯器中[建立登入頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md)的行動檢視。 無論裝置為何，都能有效傳遞您的訊息，並藉由量身打造您的內容以提升參與度，讓您在行動中輕鬆使用。 此功能將在發行後的一週內逐步推出。

[&#x200B; — 登陸頁面逐步解說影片 — &#x200B;](https://youtu.be/aPQHlG2X6c0)

**新REST API呼叫**

潛在客戶與活動REST API的三次新呼叫：

* 刪除銷售機會
* 依計畫ID取得銷售機會
* 取得已刪除的銷售機會

此外，Sync Lead也有新選項，可非同步寫入潛在客戶變更，以加快API呼叫速度。 發行後，完整詳細資料將可在[https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/home](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/home)取得

**電子郵件指令碼自訂物件支援**

現在，您可以從電子郵件指令碼中存取與帳戶物件相關聯的自訂物件！

## 即時Personalization {#real-time-personalization}

**Google和[!DNL Facebook]**&#x200B;的個人化再行銷

再行銷會向造訪過您網站的人顯示廣告。 您現在可以使用即時Personalization中的資料，在[Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)和[[!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)上個人化您的再行銷活動。 向不同產業的受眾、指定的帳戶清單、公司規模或任何已知潛在客戶的資料進行再行銷。

[具名帳戶清單模組](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

「指定帳戶」模組的增強功能將改善使用者的符合率和驗證。 新增專案包括：

* 使用潛在客戶的電子郵件地址比對「具名帳戶」清單中的組織（也適用於RTP客戶）
* 支援每個帳戶最多10萬筆記錄
* 要檢視和下載的CSV檔案範本

![](assets/image2015-1-14-11-3a12-3a16.png)

**已更新RTP標籤選項**

「帳戶設定」下的「RTP標籤」選項已更新為包含：

1. CDN和非同步（建議標籤）
1. CDN和同步（高速）
1. 不含CDN的非同步標籤
1. 不含CDN的同步標籤

為獲得最佳效能，建議在`<head>`之後將標籤放在網頁標題的頂端。 所有標籤都允許使用[RTP API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation)。 如需如何部署RTP標籤的詳細資訊，請參閱[這裡](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

![](assets/image2015-1-15-13-3a30-3a45.png)
