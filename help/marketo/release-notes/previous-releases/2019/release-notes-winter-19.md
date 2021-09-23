---
unique-page-id: 17727823
description: 發行說明 — 19年冬季 — Marketo檔案 — 產品檔案
title: 發行說明 — 2019年冬季
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 發行說明：』19年冬季 {#release-notes-winter}

』19年冬季發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

請按一下標題連結，檢視每項功能的詳細文章（若有）。

>[!NOTE]
>
>Facebook現在需要Business Manager帳戶，才能運用自訂對象整合。 您的Facebook LaunchPoint服務&#x200B;*必須*&#x200B;與Business Manager帳戶相關聯，或&#x200B;**您的整合在2019年1月14日後將無法繼續運作。** 要設定Business Manager帳戶，請參閱[Facebook幫助](https://www.facebook.com/business/help/1710077379203657)。

>[!NOTE]
>
>Microsoft正在推動所有線上客戶升級至最新版的Microsoft Dynamics。 如果您要將Marketo執行個體與Dynamics Online整合，在2019年1月31日&#x200B;**之前[升級至最新版的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)，以確保您的整合能繼續運作。**

>[!NOTE]
>
>Marketo正在將GoTo網路研討會的OAuth版本從1.0升級至2.0。OAuth 1.0的支援將於2019年1月汰除。 如果您是GoTo網路研討會客戶，您需要在2019年1月31日前&#x200B;****&#x200B;透過LaunchPoint（位於管理區域）重新驗證登入，以確保整合能持續運作。 如需更多詳細資訊，請參閱我們的[社群頁面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)。

## 核心平台增強功能 {#core-platform-enhancements}

**[適用於Marketo電子郵件的Email CC](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

在透過Marketo傳送的電子郵件中，每位收件者包含最多五個CC位址。

**API**

* **資產API的多品牌化網域支援：** 核准和複製資產會在API和UI中產生相同的結果。
* **適用於資產API的電子郵件CC支援**:透過API複製、核准和處理電子郵件的使用者，將會與UI設定保持同等。

**[Munchkin v155（測試版）](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **僅限API模式**:使用者現在可以決定追蹤其資料庫成員的時間和方式，方法是允許單頁網頁應用程式在想要記錄網頁造訪時明確呼叫，而非依賴Marketo的自動追蹤。
* **退出管理**:比對選擇退出Cookie網域與Munchkin追蹤Cookie網域，輕鬆管理選擇退出。
* **網域層級決策器參數**:雙字母網域(即「  [website.io](https://website.io)」)將在Marketo中自動追蹤，不需其他設定需求。

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce自訂設定檔**:Sales Engage現在支援無限制的自訂設定檔。

* **Salesforce自訂**:通過刪除非關鍵的自定義活動欄位，用戶可以更高效地在CRM平台中設定「銷售參與」。
* **電子郵件服務**:通過連接到Microsoft Outlook（通過Office365或通過「電子郵件連接」頁簽進行內部部署），享受更好的傳遞能力，以及改進的回復跟蹤、排程電子郵件功能和批量電子郵件功能。
* **新管理設定**:已新增兩個管理頁面，以最佳化您的Sales Engage例項

   * _團隊_ 管理可讓管理員編輯訂閱和團隊，以支援順暢的帳戶設定程式。
   * _Salesforce Admin_ Settingshelps團隊以前所未有的速度更輕鬆地設定其SFDC同步。

* **適用於Windows的OWA插件**:通過一個插件，Sales Engage將支援所有Windows Office365客戶端，從而能夠在Outlook中使用即時源。新外掛程式將可在Microsoft Store中使用。
* **活動推動者**:同步銷售參與到核心的Marketo平台，以運用即時行銷分析。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky發行的頻率較高。 預計第4季末/第1季初會推出下列功能和增強功能。 如需更多詳細資訊和更新，請查看[Sky檔案](https://help.marketo.com/)。

* **選用的預設體驗**:Marketo使用者若已由管理員提供存取權，可將Marketo Sky設為預設體驗。

* **重新想像我的Marketo**:新增小工具來自訂您的體驗，該小工具可提供重要資訊、通知和最常造訪區域的連結。

* **Design Studio清單視圖和詳細資訊頁**:透過可篩選及搜尋的電子郵件、登錄頁面和表單清單檢視，享受更高的組織層級和準確性。資產詳細資料頁面提供每個資產的重要資訊，包括資產所使用的程式、所使用的片段數量等。

* **全域搜尋**:Marketo現在提供更快速、更強大的全域搜尋功能。搜尋查詢現在會在所有可存取的工作區間執行，並可搜尋資產（使用中和已封存）、標籤、促銷活動和方案。 搜尋結果會透過覆蓋提供，而每個結果都包含其檔案位置追蹤，以指定資產的存留位置。

* **改善的使用者介面**:新的圖示、模組和按鈕，以及新的調色盤，可反映我們的品牌更新，讓Marketo Sky更令人驚嘆且更實用。

* **電子郵件計畫可用性增強**:我們持續致力於在傳統的Marketo銷售機會管理平台與新的Marketo Sky體驗之間，實現電子郵件計畫功能的同等目標。
* **含活動網路研討會計畫**:現在提供Marketo Sky式「活動結合網路研討會」課程(注意：此版本僅支援GoTo網路研討會，並隨著時間推移進一步建立整合)。

## 帳戶型行銷 {#account-based-marketing}

**[基於ABM Persona的細分和過濾](/help/marketo/product-docs/target-account-management/using-personas.md)**

針對指定帳戶中的特定角色個人化您的ABM行銷活動。 「ABM角色」功能會根據潛在客戶細分建立預設職務，並允許配置其他角色細分。

## Analytics {#analytics}

**Bizible**

* **自訂計算欄位**:使用任何Bizible屬性來建立可用於控制面板報告和細分的自訂欄位。

* **SOC II II類認證**:新的安全性和隱私認證以今年早些時候的I類認證為基礎。

## 網頁個人化 {#web-personalization}

**[在帳戶設定中新增子網域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

為了更有效率地管理網域和子網域，使用者現在可以將子網域新增至其RTP帳戶設定。

## Marketo行動參與(MME) {#marketo-mobile-engagement-mme}

**更新適用於Android的MME軟體開發套件(SDK)**

我們已將Android適用的SDK更新為更現代、穩定且可擴充的架構，其中包含更多彈性和新的工程功能。 Android應用程式開發人員現在可以透過這個新SDK直接使用Google的[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)(FCM)。

* [開發人員指示](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開發人員常見問題集](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>應用程式開發人員&#x200B;**必須**&#x200B;在2019年3月31日之前更新至新版本。 如果您在2019年3月31日前未更新SDK，在此日期後下載您應用程式的任何新使用者，在您更新至最新版SDK之前，將無法收到推播通知。 SDK更新將不需要您目前的行動應用程式使用者重新下載新版應用程式。

## 其他更新 {#additional-updates}

**可延伸網路研討會平台**

除了我們的產品版本外，我們的合作夥伴團隊正在開發新的架構，讓網路研討會提供者可建置和維護自己與Marketo的整合，在更新和增強解決方案方面提供更大的彈性，同時讓行銷人員能充分運用他們所選擇的整合。

我們計畫逐案推出新平台，由提供者提供。 如需詳細資訊，請參閱我們的[程式詳細資訊](https://www.marketo.com/why-marketo/partners/technology/)，或聯絡您的Marketo連絡人。
