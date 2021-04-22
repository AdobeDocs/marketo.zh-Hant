---
unique-page-id: 4720758
description: 發行說明- 2015年1月-Marketo文檔——產品文檔
title: 發行說明- 2015年1月
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 發行說明：2015年1月{#release-notes-january}

2015年1月發行包含下列功能。 請查看您的Marketo版以瞭解功能的可用性。 在發行後，請務必回來尋找每個功能的詳細文章連結！

## 行銷自動化更新{#marketing-automation-updates}

**適用於行動裝置的著陸頁面**

您現在可以從著陸頁面編輯器中，為著陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md)建立行動檢視。 [不論使用何種裝置，您都能有效傳遞訊息，並透過量身打造內容以方便在外出時使用，進而提升參與度。 此功能將在發行後的一週內逐步推出。

[-著陸頁面逐步影片-](https://youtu.be/aPQHlG2X6c0)

**新的Rest API呼叫**

對Lead &amp; Activity ReST API的三個新呼叫：

* 刪除銷售線索
* 依計畫ID取得銷售機會
* 獲取已刪除的銷售線索

此外，「同步銷售機會」有新的選項，可以非同步地寫入銷售機會變更，以加快API呼叫的速度。 在[developers.marketo.com](https://developers.marketo.com)發行後，將提供完整的詳細資訊

**電子郵件指令碼自訂物件支援**

現在，從電子郵件指令碼中存取與Account物件關聯的自訂物件！

## 即時個人化{#real-time-personalization}

**Google和Facebook的個人化再行銷**

再行銷會向造訪過您網站的人顯示廣告。 您現在可以使用即時個人化的資料，在[Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)和[Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)上個人化您的再行銷宣傳。 重新行銷給來自不同產業的受眾，包括具名的帳戶清單、公司規模或任何來自已知銷售機會的資料。

[命名帳戶清單模組](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

「命名帳戶」模組的增強功能將改善使用者的比對率和驗證。 新增功能包括：

* 使用Lead的電子郵件地址（也適用於RTP僅限客戶），從您的「指名帳戶」清單中比對組織
* 支援每個帳戶最多10萬個記錄
* 檢視和下載CSV檔案範本

![](assets/image2015-1-14-11-3a12-3a16.png)

**更新的RTP標籤選項**

「Account Settings（帳戶設定）」下的RTP標籤選項已更新為包括：

1. CDN和非同步（建議的標籤）
1. CDN與同步（高速）
1. 不需CDN的非同步標籤
1. 不需CDN的同步標籤

為獲得最佳效能，建議將標籤放置在`<head>`之後網頁頁首的頂端。 所有標籤都允許使用[RTP API](https://developers.marketo.com/documentation/websites/rtp-js-api/)。 有關如何部署RTP標籤的資訊，請參見[此處](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

![](assets/image2015-1-15-13-3a30-3a45.png)
