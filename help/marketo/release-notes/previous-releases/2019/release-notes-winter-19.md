---
unique-page-id: 17727823
description: 發行說明 — 冬季』19年 — Marketo檔案 — 產品檔案
title: 發行說明 — 2019年冬季
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 0%

---

# 發行說明： Winter &#39;19 {#release-notes-winter}

以下功能包含在2019年冬季發行版本中。 檢查您的Marketo版本是否有功能可用。

請按一下標題連結，檢視每個功能的詳細文章（若有）。

>[!NOTE]
>
>facebook現在需要Business Manager帳戶才能運用您的自訂對象整合。 您的Facebook LaunchPoint服務&#x200B;*必須*&#x200B;與Business Manager帳戶相關聯，或&#x200B;**您的整合在2019年1月14日之後將不再有效**。 若要設定Business Manager帳戶，請參閱[Facebook說明](https://www.facebook.com/business/help/1710077379203657)。

>[!NOTE]
>
>Microsoft正推動所有線上客戶升級至Microsoft Dynamics最新版本。 如果您正在整合Marketo執行個體與Dynamics Online，您必須在&#x200B;**2019年1月31日**&#x200B;之前[升級到最新版本的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)，以確保您的整合可繼續運作。

>[!NOTE]
>
>Marketo正在將GoToWebinar的OAuth版本從1.0升級至2.0。對OAuth 1.0的支援將於2019年1月終止支援。 如果您是GoToWebinar客戶，您必須在&#x200B;**2019年1月31日**&#x200B;前，透過LaunchPoint （在管理區域中）重新驗證您的登入，以確保您的整合可繼續運作。 如需詳細資訊，請參閱我們的[社群頁面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)。

## 核心平台增強功能 {#core-platform-enhancements}

**[Marketo電子郵件的電子郵件副本](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

在透過Marketo傳送的電子郵件中，每個收件者最多包含五個副本抄送地址。

**API**

* **資產API的多品牌網域支援：**&#x200B;核准和複製資產會在API和UI中產生相同的結果。
* **資產API的電子郵件CC支援**：使用者透過API複製、核准及處理電子郵件，將能維持與UI設定的同等性。

**[Munchkin v155 (Beta)](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking)**

* **僅限API模式**：使用者現在可以決定何時及如何追蹤其資料庫成員，方法為允許單頁網頁應用程式在想要記錄網頁造訪時明確呼叫，而非依賴Marketo的自動追蹤。
* **選擇退出管理**：將選擇退出Cookie網域與Munchkin追蹤Cookie網域比對，以輕鬆管理選擇退出。
* **網域層級決定程式引數**：兩個字母的網域（即「[website.io](https://website.io)」）將在Marketo中自動追蹤，不需要額外的設定需求。

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce自訂設定檔**： Sales Engage現在支援無限制的自訂設定檔。

* **Salesforce自訂**：透過移除非關鍵性自訂活動欄位，使用者可以更有效率地設定CRM平台中的Sales Engage。
* **電子郵件服務**：透過連線至Microsoft Outlook （透過Office365或透過[電子郵件連線]索引標籤在內部部署），享受更優異的傳遞能力，以及更優異的回覆追蹤、排程電子郵件功能和大量電子郵件功能。
* **新的管理員設定**：已新增兩個管理員頁面，以最佳化您的Sales Engage執行個體

   * _團隊管理_&#x200B;允許管理員編輯訂閱和團隊，支援順暢的帳戶設定程式。
   * _Salesforce管理設定_&#x200B;可協助團隊更快速且更輕鬆地設定SFDC同步處理。

* **適用於Windows的OWA外掛程式**：透過單一增益集，所有Windows Office365使用者端將可支援Sales Engage，提供在Outlook中使用即時摘要的功能。 新的外掛程式可在Microsoft商店中使用。
* **活動推播程式**：將銷售參與同步處理至核心Marketo平台，以運用即時行銷深入分析。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky發行會更頻繁地進行。 下列功能和增強功能預計會在第4季後期/第1季初期發行。 如需詳細資訊和更新，請參閱我們的[Sky檔案](https://help.marketo.com/)。

* **選用的預設體驗**：如果管理員已提供Marketo使用者的存取權，則他們可將Marketo Sky設定為其預設體驗。

* **重新想像我的Marketo**：新增提供重要資訊、通知和您最常造訪區域連結的Widget，以自訂您的體驗。

* **Design Studio清單檢視與詳細資料頁面**：透過可篩選及可搜尋的電子郵件、登入頁面及表單清單檢視，享受更高的組織等級與正確性。 資產詳細資料頁面提供關於每個資產的重要資訊，包括資產使用的程式、使用的程式碼片段數量等。

* **全域搜尋**： Marketo現在可在整個平台提供更快速、更強大的全域搜尋功能。 搜尋查詢現在會在所有可存取的工作區中執行，並且可以搜尋資產（使用中及已封存）、標籤、行銷活動和方案。 搜尋結果會透過覆蓋圖提供，每個結果都包含其檔案位置軌跡，以指定資產所在的位置。

* **改善的使用者介面**：新的圖示、模式和按鈕，以及新的調色盤，可反映我們的品牌更新，讓Marketo Sky更令人驚豔且功能更強大。

* **電子郵件方案可用性增強功能**：我們持續邁向傳統Marketo銷售機會管理平台與新Marketo Sky體驗之間的電子郵件方案功能對等化。
* **具有網路研討會程式**：具有網路研討會程式Marketo Sky現已推出（注意：此版本僅支援GoToWebinar，並會隨著時間建立進一步的整合）。

## Account-Based Marketing {#account-based-marketing}

**[ABM角色型細分與篩選](/help/marketo/product-docs/target-account-management/using-personas.md)**

為指定帳戶中的特定角色個人化ABM行銷活動。 ABM角色功能會根據潛在客戶細分建立預設職稱，並允許設定其他角色細分。

## Analytics {#analytics}

**Bizible**

* **自訂計算欄位**：使用任何Bizible屬性來建置可用於儀表板報告和分段的自訂欄位。

* **SOC II Type II Certification**：新的安全性與隱私權認證是以今年早些時候的Type I認證為基礎。

## 網頁Personalization {#web-personalization}

**[在帳戶設定中新增子網域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

為了更有效率地管理網域和子網域，使用者現在可以將子網域新增至其RTP帳戶設定。

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**已更新Android的MME軟體開發套件(SDK)**

我們已將Android的SDK更新為更現代、穩定且可擴展的架構，其中包含更多彈性和新的工程功能。 Android應用程式開發人員現在可以直接將Google的[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM)與此新SDK搭配使用。

* [開發人員指示]https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)

>[!NOTE]
>
>應用程式開發人員&#x200B;**必須**&#x200B;在2019年3月31日之前更新為新版本。 如果您未在2019年3月31日之前更新SDK，任何在此日期後下載您的應用程式的新使用者，將無法收到推播通知，直到您更新至最新版SDK為止。 SDK更新不需要您目前的行動應用程式使用者重新下載新版的應用程式。

## 其他更新 {#additional-updates}

**可擴充網路研討會平台**

除了我們的產品發行外，我們的合作夥伴團隊正在研究新的架構，此架構可讓網路研討會提供者建立並維護他們與Marketo的整合，提供更大彈性來更新及增強其解決方案，同時讓行銷人員能夠充分運用他們所選的整合。

我們計畫根據個別情況，向提供者推出我們的新平台。 如需詳細資訊，請參閱我們的[方案詳細資料](https://www.marketo.com/why-marketo/partners/technology/)或聯絡您的Marketo連絡人。
