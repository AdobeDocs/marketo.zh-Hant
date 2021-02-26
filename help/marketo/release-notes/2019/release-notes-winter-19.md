---
unique-page-id: 17727823
description: 發行說明- 19年冬季——行銷檔案——產品檔案
title: 發行說明- 19年冬季
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---


# 發行說明：冬季&#39;19 {#release-notes-winter}

Winter &#39;19版本包含下列功能。 檢查您的Marketo版本，以取得功能。

請按一下標題連結，檢視每個功能的詳細文章（如果有的話）。

>[!NOTE]
>
>Facebook現在需要Business Manager帳戶，才能運用您的自訂對象整合。 您的Facebook LaunchPoint服務&#x200B;*必須*&#x200B;與Business Manager帳戶關聯，否則您的整合在2019年1月14日後將無法運作。 ****&#x200B;若要設定Business Manager帳戶，請參閱[Facebook說明](https://www.facebook.com/business/help/1710077379203657)。

>[!NOTE]
>
>Microsoft正在推動所有線上客戶升級至最新版Microsoft Dynamics。 如果您要將Marketo實例與Dynamics Online整合，您將需要[在2019年1月31日&#x200B;**之前升級至最新版的Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md)，以確保您的整合能繼續運作。**

>[!NOTE]
>
>Marketo正在將GoTo網路研討會的OAuth版本從1.0升級至2.0。2019年1月將不再支援OAuth 1.0。 如果您是GoToWebinar客戶，您將需要在2019年1月31日&#x200B;****&#x200B;之前，透過LaunchPoint（在「管理員」區域）重新驗證登入，以確保您的整合能繼續運作。 如需詳細資訊，請參閱[社群頁面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)。

## 核心平台增強功能{#core-platform-enhancements}

**[適用於行銷人員的電子郵件CC](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

透過Marketo傳送的電子郵件中，每個收件者最多可包含5個CC位址。

**API**

* **資產API的多品牌網域支援：核** 準和仿製資產會在API和UI中產生相同的結果。
* **資產API的電子郵件CC支援**:使用者透過API複製、核准和處理電子郵件時，會維持與UI設定的相同性。

**[Munchkin v155(Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **僅API模式**:使用者現在可決定追蹤其資料庫成員的時機和方式，允許單頁網頁應用程式在他們想要記錄網頁瀏覽時明確呼叫，而非依賴Marketo的自動追蹤。
* **退出管理**:將退出Cookie網域與Munchkin追蹤Cookie網域相符，輕鬆管理退出。
* **網域層級決策者參數**:雙字母網域(即&quot;  [website.io](https://website.io)&quot;)將自動在Marketo中追蹤，而不需額外的設定要求。

## Marketo銷售人員參與{#marketo-sales-engage}

* **Salesforce自訂設定檔**:Sales Engage現在支援無限制的自訂個人檔案。

* **Salesforce自訂**:借由移除非關鍵的自訂活動欄位，使用者可以更有效率地設定CRM平台中的「銷售參與」。
* **電子郵件服務**:透過連線至Microsoft Outlook（透過Office365或「電子郵件連線」標籤的「預先安裝」），體驗更佳的傳遞能力，以及改良的回覆追蹤、排程電子郵件功能和大量電子郵件功能。
* **新管理員設定**:已新增兩個管理頁面，以最佳化您的「銷售參與」例項

   * _Team_ Management可讓管理員編輯訂閱和團隊，以支援順暢的帳戶設定程式。
   * _Salesforce管理_ 員設定Shelps團隊以前所未有的快速輕鬆方式設定其SFDC同步。

* **OWA Plugin for Windows**:只需單一附加元件，所有Windows Office365客戶端都將在Sales Engage中受到支援，從而能夠在Outlook中使用即時動態消息。新增外掛程式將可在Microsoft Store中使用。
* **活動推動者**:同步銷售與核心行銷人員互動以運用即時行銷見解。

## Marketo Sky{#marketo-sky}

>[!NOTE]
>
>Marketo Sky釋放會以更頻繁的節奏發生。 下列功能和增強功能預計將於第4季末／第1季初推出。 如需詳細資訊和更新，請查看我們的[Sky檔案](https://help.marketo.com/)。

* **可選預設體驗**:Marketo使用者若已由管理員提供存取權，可將Marketo Sky設定為預設體驗。

* **重新改良我的行銷工具**:新增Widget，提供重要資訊、通知和最常造訪區域的連結，以自訂您的體驗。

* **Design Studio清單檢視與詳細資訊頁面**:透過可填寫且可搜尋的電子郵件、登陸頁面和表單清單檢視，體驗更高的組織與精確度。「資產詳細資料頁面」提供每個資產的關鍵資訊，包括資產所使用的程式、所使用的程式碼片段數等。

* **全域搜尋**:Marketo現在提供更快速、更強穩的全域平台搜尋功能。搜尋查詢現在可在所有可存取的工作區中執行，並可搜尋資產（活動中和封存）、標籤、促銷活動和程式。 搜尋結果會透過覆蓋提供，而每個結果都包含其檔案位置記錄，以指定資產的存留位置。

* **改良的使用者介面**:全新的圖示、樣式和按鈕，以及全新的調色盤，以反映我們的品牌更新效果，讓Marketo Sky更令人驚艷和功能更強大。

* **電子郵件計畫可用性增強**:我們繼續邁向「電子郵件計畫」功能的平等化，將我們傳統的「行銷線索管理」平台與新的Marketo Sky體驗結合在一起。
* **網路研討會活動計畫**:現在提供包含網路研討會的活動方案，包括Marketo Sky(注意：本版本僅支援GoToWebinar，並隨著時間推移進一步整合)。

## 帳戶型行銷{#account-based-marketing}

**[基於ABM人格的細分與過濾](/help/marketo/product-docs/account-based-marketing/using-personas.md)**

針對指定帳戶中的特定角色個人化您的ABM宣傳。 「ABM角色」功能會根據銷售機會細分建立預設職銜，並允許設定其他角色細分。

## Analytics {#analytics}

**比齊布爾**

* **自訂計算欄位**:使用任何Bizible屬性來建立可用於控制面板報告和區段的自訂欄位。

* **SOC II II類認證**:新的安全性和隱私權認證以今年早些時候的I類認證為基礎。

## Web個人化{#web-personalization}

**[在帳戶設定中新增子網域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

為了更有效率地管理網域和子網域，使用者現在可以將子網域新增至其RTP帳戶設定。

## Marketo Mobile參與(MME){#marketo-mobile-engagement-mme}

**更新的Android MME軟體開發套件(SDK)**

我們已將適用於Android的SDK更新為更現代化、穩定且可擴充的架構，其中包含更多彈性和新的工程功能。 Android應用程式開發人員現在可以直接將Google的[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/)(FCM)與這個新的SDK搭配使用。

* [開發人員指示](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開發人員常見問答集](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>應用程式開發人員&#x200B;**必須**&#x200B;在2019年3月31日之前更新至新版本。 如果您未在2019年3月31日之前更新SDK，在此日期之後下載您應用程式的任何新使用者，在您更新至最新版SDK之前，將無法收到推播通知。 SDK更新將不需要您目前的行動應用程式使用者重新下載新版本的應用程式。

## 其他更新{#additional-updates}

**可擴充的網路研討會平台**

除了我們的產品版本外，我們的合作夥伴團隊還在建立新的架構，讓網路研討會供應商能夠建立並維護與Marketo的整合，提供更靈活的更新和增強解決方案，同時讓行銷人員充份運用其選擇的整合。

我們計畫逐案推出與供應商合作的新平台。 如需詳細資訊，請參閱我們的[程式詳細資訊](https://www.marketo.com/why-marketo/partners/technology/)，或聯絡您的行銷人員聯絡。
