---
unique-page-id: 17727823
description: 發行說明 — 冬季』19 - Marketo檔案 — 產品檔案
title: 發行說明 — Winter 』19年
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 發行說明： Winter 』19年 {#release-notes-winter}

以下功能包含在2019年冬季發行版本中。 檢視您的Marketo版本，瞭解是否有功能可用。

請按一下標題連結，檢視每個功能的詳細文章（若有）。

>[!NOTE]
>
>facebook現在需要Business Manager帳戶，才能運用您的自訂對象整合。 您的Facebook LaunchPoint服務 *必須* 與Business Manager帳戶相關聯或 **2019年1月14日後，您的整合將不再運作**. 若要設定業務管理員帳戶，請參閱 [facebook說明](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft正在推動所有線上客戶升級至Microsoft Dynamics的最新版本。 如果您要將Marketo執行個體與Dynamics Online整合，您需要 [升級至最新版Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) 早於 **2019年1月31** 以確保您的整合可繼續運作。

>[!NOTE]
>
>Marketo正在將GoToWebinar的OAuth版本從1.0升級至2.0。對OAuth 1.0的支援將於2019年1月汰除。 如果您是GoToWebinar客戶，您必須透過LaunchPoint （在「管理員」區域）重新驗證登入，驗證方式如下 **2019年1月31** 以確保您的整合可繼續運作。 如需更多詳細資料，請參閱我們的 [社群頁面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## 核心平台增強功能 {#core-platform-enhancements}

**[Marketo電子郵件的電子郵件副本](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

透過Marketo傳送的電子郵件中，每個收件者最多可包含五個副本地址。

**API**

* **資產API的多品牌網域支援：** 核准和複製資產會在API和UI中產生相同的結果。
* **Asset API的電子郵件CC支援**：使用者透過API複製、核准和處理電子郵件時，將維持與UI設定的對等性。

**[Munchkin v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **僅限API模式**：使用者現在可以決定何時及如何追蹤其資料庫成員，方法為允許單頁網頁應用程式在想要記錄網頁瀏覽時明確呼叫，而非仰賴Marketo的自動追蹤。
* **選擇退出管理**：比對選擇退出Cookie網域與Munchkin追蹤Cookie網域，輕鬆管理選擇退出。
* **網域層級決策程式引數**：兩個字母的網域(即&quot; [website.io](https://website.io)&quot;)會自動在Marketo中追蹤，不需要額外的設定要求。

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce自訂設定檔**：Sales Engage現在支援無限制的自訂設定檔。

* **Salesforce自訂**：透過移除非關鍵自訂活動欄位，使用者可以更有效率地設定Sales Engage in the CRM平台。
* **電子郵件服務**：透過連線至Microsoft Outlook （透過Office365或透過「電子郵件連線」索引標籤內部部署），享受更優異的可遞送性，以及改進的回覆追蹤、排程電子郵件功能和大量電子郵件功能。
* **新增管理員設定**：已新增兩個管理員頁面，以最佳化您的Sales Engage執行個體

   * _團隊管理_ 允許管理員編輯訂閱和團隊，支援順暢的帳戶設定程式。
   * _Salesforce管理設定_ 協助團隊設定SFDC同步處理比以往更快更輕鬆。

* **適用於Windows的OWA外掛程式**：透過單一增益集，所有Windows Office365使用者端都可在Sales Engage中取得支援，讓您能夠在Outlook中使用即時摘要。 新的外掛程式將可在Microsoft市集使用。
* **活動推送程式**：將Sales Engage同步至核心Marketo平台，以運用即時行銷分析。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky發行會更頻繁地進行。 下列功能和增強功能預計會在第4季末/第1季初發佈。 如需詳細資訊和更新，請檢視我們的 [Sky檔案](https://help.marketo.com/).

* **選用的預設體驗**：如果管理員已提供Marketo使用者的存取權，他們可將Marketo Sky設定為其預設體驗。

* **重新想像我的Marketo**：新增Widget來自訂您的體驗，提供重要資訊、通知，以及您最常造訪區域的連結。

* **Design Studio清單檢視和詳細頁面**：透過可篩選和可搜尋的電子郵件、登陸頁面和表單清單檢視，享受更高級別的組織和準確性。 資產詳細資料頁面提供有關每個資產的重要資訊，包括資產使用哪些程式、使用的代碼片段數量等等。

* **全域搜尋**：Marketo現在會在整個平台上提供更快、更強大的全域搜尋功能。 搜尋查詢現在會在所有可存取的工作區中執行，並可搜尋資產（使用中及已封存）、標籤、行銷活動和方案。 搜尋結果會透過覆蓋圖提供，每個結果都包含其檔案位置軌跡，以指定資產所在的位置。

* **改善的使用者介面**：新的圖示、模式和按鈕，以及新的調色盤，可反映我們的品牌更新，並使Marketo Sky更令人驚豔和實用。

* **電子郵件計畫可用性增強功能**：我們繼續邁向在傳統Marketo銷售機會管理平台與新Marketo Sky體驗之間實現電子郵件計畫功能對等的目標。
* **網路研討會活動計畫**：具有網路研討會的計畫現在可在Marketo Sky中使用（注意：此版本僅支援GoToWebinar，並會隨著時間建立進一步整合）。

## Account-Based Marketing {#account-based-marketing}

**[ABM角色型細分與篩選](/help/marketo/product-docs/target-account-management/using-personas.md)**

為指定帳戶中的特定角色個人化ABM行銷活動。 ABM角色功能會根據潛在客戶細分建立預設職稱，並允許設定其他角色細分。

## Analytics {#analytics}

**Bizible**

* **自訂計算欄位**：使用任何Bizible屬性來建立可用於控制面板報告和分段的自訂欄位。

* **SOC II Type II認證**：新的安全性和隱私權認證是以今年早些時候的I類認證為基礎。

## 網頁個人化 {#web-personalization}

**[在帳戶設定中新增子網域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

為了更有效率地管理網域和子網域，使用者現在可以將子網域新增到其RTP帳戶設定。

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**更新適用於Android的MME軟體開發套件(SDK)**

我們已將Android適用的SDK更新為更現代、更穩定且可擴展的架構，其中包含更多彈性和新的工程功能。 Android應用程式開發人員現在可以直接使用Google的 [Firebase雲端通訊](https://firebase.google.com/docs/cloud-messaging/) (FCM)搭配此新SDK。

* [開發人員指示](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開發人員常見問題集](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>應用程式開發人員 **必須** 在2019年3月31日之前更新至新版本。 如果您未在2019年3月31日之前更新SDK，任何在此日期後下載您應用程式的新使用者，將無法收到推播通知，直到您更新至最新版SDK為止。 SDK更新不會要求您目前現有的行動應用程式使用者重新下載新版的應用程式。

## 其他更新 {#additional-updates}

**可延伸網路研討會平台**

除了我們的產品發行外，我們的合作夥伴團隊正在研究新的架構，此架構可讓網路研討會提供者建立和維護他們與Marketo的整合，提供更大彈性來更新及增強其解決方案，同時讓行銷人員充分運用他們選擇的整合。

我們計畫根據個別案例，與提供者共同推出新平台。 如需詳細資訊，請參閱我們的 [方案詳細資料](https://www.marketo.com/why-marketo/partners/technology/) 或聯絡您的Marketo聯絡人。
