---
title: 2019
description: 2019 - Marketo檔案 — 產品檔案
feature: Release Information
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: d5c7388a-594e-4d15-9b39-98d6ce479e8bid: de9e3aa9-f002-4fe1-897b-09ee3c55114bid: df8eb12b-4f82-491f-acbb-d74012ca5654id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bbbea26f-9621-49eb-9ab8-e06fb3bbce8cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 4d4669f3239b43afbcbd660644c8d1a35734a556
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 0%

---

# 2019

## 2019年冬季 {#winter}

以下功能包含在2019年冬季發行版本中。 檢查您的Marketo版本是否有功能可用。

請按一下標題連結，檢視每個功能的詳細文章（若有）。

>[!NOTE]
>
>[!DNL Facebook]現在需要Business Manager帳戶才能運用您的自訂對象整合。 您的[!DNL Facebook] LaunchPoint服務&#x200B;*必須*&#x200B;與Business Manager帳戶相關聯，或&#x200B;**您的整合在2019年1月14日之後將不再運作**。 若要設定Business Manager帳戶，請參閱[[!DNL Facebook] 說明](https://www.facebook.com/business/help/1710077379203657)。

>[!NOTE]
>
>Microsoft正在推送所有線上客戶升級至[!DNL Microsoft Dynamics]的最新版本。 如果您正在整合您的Marketo執行個體與[!DNL Dynamics Online]，您需要在&#x200B;**2019年1月31日**&#x200B;之前[升級至最新版本的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)，以確保您的整合可繼續運作。

>[!NOTE]
>
>Marketo正在將GoToWebinar的OAuth版本從1.0升級至2.0。 對OAuth 1.0的支援將於2019年1月終止支援。 如果您是GoToWebinar客戶，您必須在&#x200B;**2019年1月31日**&#x200B;前，透過LaunchPoint （在管理區域中）重新驗證您的登入，以確保您的整合可繼續運作。 如需詳細資訊，請參閱我們的[社群頁面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)。

## 核心平台增強功能 {#core-platform-enhancements}

**[Marketo電子郵件的電子郵件副本](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

在透過Marketo傳送的電子郵件中，每個收件者最多包含五個副本抄送地址。

**API**

* **資產API的多品牌網域支援：**&#x200B;核准和複製資產會在API和UI中產生相同的結果。
* **資產API的電子郵件CC支援**：使用者透過API複製、核准及處理電子郵件，將能維持與UI設定的同等性。

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **僅限API模式**：使用者現在可以決定何時及如何追蹤其資料庫成員，方法為允許單頁網頁應用程式在想要記錄網頁造訪時明確呼叫，而非依賴Marketo的自動追蹤。
* **選擇退出管理**：將選擇退出Cookie網域與[!DNL Munchkin]追蹤Cookie網域比對，以輕鬆管理選擇退出。
* **網域層級決定程式引數**：兩個字母的網域（即「[website.io](https://website.io)」）將在Marketo中自動追蹤，不需要額外的設定需求。

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]自訂設定檔**： Sales Engage現在支援無限制的自訂設定檔。

* **[!DNL Salesforce]自訂**：透過移除非關鍵自訂活動欄位，使用者可以更有效率地設定CRM平台中的Sales Engage。
* **電子郵件服務**：透過連線至[!DNL Microsoft Outlook] （透過Office365或透過[電子郵件連線]索引標籤在內部部署），享受更好的傳遞能力，並改善回覆追蹤、排程電子郵件功能和大量電子郵件功能。
* **新的管理員設定**：已新增兩個管理員頁面，以最佳化您的Sales Engage執行個體

   * *團隊管理*&#x200B;允許管理員編輯訂閱和團隊，支援順暢的帳戶設定程式。
   * *Salesforce管理設定*&#x200B;可協助團隊更快且更輕鬆地設定SFDC同步處理。

* **適用於[!DNL Windows]**&#x200B;的OWA外掛程式：透過單一增益集，所有[!DNL Windows Office365]使用者端將可支援Sales Engage，因此能夠在Outlook中使用即時摘要。 新的外掛程式可在Microsoft商店中使用。
* **活動推播程式**：將銷售參與同步處理至核心Marketo平台，以運用即時行銷深入分析。

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>[!DNL Marketo Sky]發行更頻繁地進行。 下列功能和增強功能預計會在第4季後期/第1季初期發行。 如需詳細資訊和更新，請參閱我們的[Sky檔案](https://help.marketo.com/)。

* **選用的預設體驗**：如果管理員已提供存取權，Marketo使用者可將[!DNL Marketo Sky]設定為其預設體驗。

* **重新想像我的Marketo**：新增提供重要資訊、通知和您最常造訪區域連結的Widget，以自訂您的體驗。

* **Design Studio清單檢視與詳細資料頁面**：透過可篩選及可搜尋的電子郵件、登入頁面及表單清單檢視，享受更高的組織等級與正確性。 資產詳細資料頁面提供關於每個資產的重要資訊，包括資產使用的程式、使用的程式碼片段數量等。

* **全域搜尋**： Marketo現在可在整個平台提供更快速、更強大的全域搜尋功能。 搜尋查詢現在會在所有可存取的工作區中執行，並且可以搜尋資產（使用中及已封存）、標籤、行銷活動和方案。 搜尋結果會透過覆蓋圖提供，每個結果都包含其檔案位置軌跡，以指定資產所在的位置。

* **改善的使用者介面**：新的圖示、模式和按鈕，以及新的調色盤，可反映我們的品牌更新，讓[!DNL Marketo Sky]更令人驚豔且功能更強大。

* **電子郵件方案可用性增強功能**：我們持續邁向在傳統Marketo銷售機會管理平台與新的[!DNL Marketo Sky]體驗之間實現電子郵件方案功能的對等化。
* **具有網路研討會程式**：具有網路研討會程式[!DNL Marketo Sky]現已提供使用（注意：此版本僅支援GoToWebinar，並隨著時間建立進一步的整合）。

## Account-Based Marketing {#account-based-marketing}

**[ABM角色型細分與篩選](/help/marketo/product-docs/target-account-management/using-personas.md)**

為指定帳戶中的特定角色個人化ABM行銷活動。 ABM角色功能會根據潛在客戶細分建立預設職稱，並允許設定其他角色細分。

## 分析 {#analytics}

**[!DNL Bizible]**

* **自訂計算欄位**：使用任何[!DNL Bizible]屬性來建立可用於儀表板報告和分段的自訂欄位。

* **SOC II Type II Certification**：新的安全性與隱私權認證是以今年早些時候的Type I認證為基礎。

## [!DNL Web Personalization] {#web-personalization}

**[在帳戶設定中新增子網域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

為了更有效率地管理網域和子網域，使用者現在可以將子網域新增至其RTP帳戶設定。

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**已更新Android的MME Software Development Kit (SDK)**

我們已將適用於Android的SDK更新為更現代、更穩定且可擴展的架構，其中包含更多彈性和新的工程功能。 Android應用程式開發人員現在可以直接將Google的[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM)與此新的SDK搭配使用。

* [開發人員指示](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [開發人員常見問題集](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>應用程式開發人員&#x200B;**必須**&#x200B;在2019年3月31日之前更新為新版本。 如果您未在2019年3月31日之前更新SDK，則在此日期之後下載您的應用程式的任何新使用者，都將無法接收推播通知，直到您更新至最新版本的SDK為止。 SDK更新不需要您目前的行動應用程式使用者重新下載新版的應用程式。

## 其他更新 {#additional-updates}

**可擴充網路研討會平台**

除了我們的產品發行外，我們的合作夥伴團隊正在研究新的架構，此架構可讓網路研討會提供者建立並維護他們與Marketo的整合，提供更大彈性來更新及增強其解決方案，同時讓行銷人員能夠充分運用他們所選的整合。

我們計畫根據個別情況，向提供者推出我們的新平台。 如需詳細資訊，請參閱我們的[方案詳細資料](https://www.marketo.com/why-marketo/partners/technology/)或聯絡您的Marketo連絡人。

## 2019年春季 {#spring}

以下功能包含在2019年春季發行版本中。 檢查您的Marketo版本是否有功能可用。

請按一下標題連結，檢視每個功能的詳細文章（若有）。

***每季發行_**

下列功能已於2019年3月15日發行。

## 核心平台增強功能 {#core-platform-enhancements}

* **已輪候：**&#x200B;當您要[保留成員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)直到空缺開啟為止，要輪候成員的新計畫/事件狀態。 這適用於與Marketo Classic中的事件方案相關的管道，以及與[!DNL Marketo Sky]中的網路研討會方案相關的事件和事件。 依預設，「輪候」與「已註冊」的步驟值相同。
* **[自訂通訊限制](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**：管理員現在可以設定自訂每日或每週通訊限制。
* **[Smart Campaign Asset API](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**：透過更新日期和ID的智慧行銷活動記錄擷取，讓您在Marketo外部的分析更為豐富。
* **電子郵件的HTTPS追蹤連結：**&#x200B;對於已購買「追蹤連結的安全網域」的客戶，品牌追蹤連結現在可以在您的電子郵件中顯示為HTTPS。
* **電子郵件傳遞能力Powerpack更新**：能夠標幟並評論特定測試結果、透過URL與利害關係人分享結果，以及追蹤變更，以便在利害關係人編輯內容時檢視電子郵件的演變。

Account-Based Marketing

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)**&#x200B;現已正式推出。 AccountAI使用人工智慧來顯示您應該針對ABM策略鎖定的帳戶。

<br> 

**_非每季發行_**

下列功能預計會在整個第一季度和第二季初發佈。

## [!DNL Marketo Sky] {#marketo-sky}

* **完整的電子郵件程式功能**：傳送電子郵件、建立A/B測試並追蹤結果，以提供使用者友善的體驗。
* **智慧型行銷活動功能**：隨著智慧型行銷活動功能在Sky中繼續推出，讓您在新的使用者介面中享受增強的穩定性。
* **管理Design Studio Assets**：新增從Design Studio清單檢視大量管理範本、影像、Forms、代碼片段、檔案、電子郵件和登入頁面的功能。
* **在收件者時區傳遞控制面板**：瞭解客戶使用Sky中的在收件者時區傳遞功能所傳送電子郵件的報告行為。

## Marketo Sales Engage {#marketo-sales-engage}

* **增強型稽核**：在例項中，新增其他使用者建立的[結束現有行銷活動](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)的功能，以檢視所有人員、電子郵件和[內容](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md)。
* **[取消訂閱管理](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**：透過[封鎖電子郵件網域](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md)的連絡功能，最大化傳遞能力及合規性。 Marketo在傳送電子郵件之前，也會交叉參考潛在客戶資料庫以取消訂閱。

## 由Marketo進行的[!DNL Bizible] {#bizible-by-marketo}

* **[!DNL Bizible]探索功能增強功能**：新的儀表板分段功能可讓行銷人員更清楚瞭解效能。
* **多貨幣支援**：利用[!DNL Bizible]以CRM貨幣資料表為基礎的全新自動貨幣轉換功能，在您的公司貨幣與任何本幣之間切換。
* **CRM行銷活動成本**：測量離線行銷活動的支出和ROI，並自動從CRM行銷活動物件提取成本資料。

## 2019 年 6 月 {#june}

2019年6月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

**_每季發行_**

下列功能已於2019年6月14日發行。

## Marketo核心服務 {#marketo-core-services}

* **大量擷取檔案總和檢查碼**：將您的檔案雜湊與已完成擷取工作的總和檢查碼字串進行比較，以確認已擷取到完整的檔案。
* **從Email 1.0自動移轉至Email 2.0**： Email 2.0與Email 1.0電子郵件和範本完全相容。 享受新功能，例如分組內容元素（影像、文字等）的功能 在模組中，在範本中定義字串、顏色、影像等變數，並利用完全回應的入門範本。 也包含視覺化電子郵件範本選擇器。

>[!CAUTION]
>
>自2019年6月18日起，不再提供Email 1.0。 您可以在[此處](https://nation.marketo.com/docs/DOC-7038)進一步瞭解Email 2.0和Email 1.0的淘汰。

## Account-Based Marketing {#account-based-marketing}

* **[!DNL LinkedIn]帳戶比對(BETA)** ：測試版現在提供新的ABM功能，讓您能夠直接從Marketo將已知和空白帳戶清單傳送至LinkedIn。 此功能會自動納入所有Marketo ABM客戶中。

<br> 

**_整個季度發行_**

下列功能預計會在整個第二行事曆季度並持續至2019年第三季初。

## [!DNL Marketo Sky] {#marketo-sky}

* **事件上限**&#x200B;和&#x200B;**事件目標**&#x200B;通常可在[!DNL Marketo Sky]中的Premium Events附加元件下取得。

   * 事件上限：使用註冊上限、頁面重新導向和輪候表功能，最佳化您活動和網路研討會的客戶體驗。
   * 活動目標：設定活動註冊和出席目標並即時追蹤進度。

* **完整導覽連結**：我們已啟用導覽至所有授權的應用程式，例如Hootsuite、Calendar等。
* **電子郵件、登陸頁面、程式碼片段、表單、影像和檔案清單檢視**：在Design Studio中檢視、搜尋您的任何資產，並對這些資產採取大量動作。
* **影像、檔案和程式碼片段詳細資料頁面**：取得您資產的快速詳細資訊，其中含有中繼資料（例如&#x200B;_在/由_&#x200B;建立）以及動作（例如&#x200B;_刪除_&#x200B;和&#x200B;_核准_）。
* **社群部落格貼文Widget**：存取Marketo中社群的最近貼文。
* **即將到期的Widget**：將「即將到期」Widget新增至您的「我的Marketo」儀表板，以檢視哪些促銷活動和登入頁面設定為下次到期。
* **更多智慧清單卡**：使用其他智慧清單卡適當地劃分割槽段和目標位置，包括「建立工作」流程步驟、CRM智慧清單規則等。
* **電子郵件Champion/Challenger詳細資訊頁面**：檢視您的電子郵件Champion/Challenger測試中的成功標準、建立時間等資料。

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* **在[!DNL Salesforce]自訂中的大量動作**：透過[!DNL Salesforce]自訂大量傳送電子郵件並新增連絡人至行銷活動，以最大化生產力。
* **設定 — [!DNL Salesforce]管理員與非管理員頁面**：透過與[!DNL Sales Connect]連線的[!DNL Salesforce]執行個體的清晰檢視以及我的電子郵件至[!DNL Salesforce]更新，管理您的[!DNL Sales Connect]執行個體。 未來幾個月將推出管理員、非管理員和Team Wide Sync的增強同步設定。
* **設定 — 整合頁面**：提供所有整合服務的一站式商店，讓您充分利用我們開放的生態系統。
* **設定 — 設定檔頁面**：檢視並更新您的帳戶詳細資料、變更密碼，以及檢查您執行個體在此新設定檔頁面上的實作狀態。

* **系統電子郵件範本**：更新設計、回應能力和國際化功能。

## 由Marketo進行的[!DNL Bizible] {#bizible-by-marketo}

* **[!DNL Dynamics]**&#x200B;的多重貨幣支援： [!DNL Bizible]現在可調整為[!DNL Microsoft Dynamics]貨幣表格，因此您可以輕鬆切換公司貨幣與當地貨幣。 （注意：對SFDC的支援已於2019年第1季度發行。）
* **漂移整合**：瞭解漂移對話如何影響客戶的歷程。 [!DNL Bizible]也會從交談中擷取電子郵件地址，以建立新的銷售機會，或將接觸點連線到現有的銷售機會。
* **本地化**： [!DNL Bizible]現在提供所有Marketo支援的語言（英文、日文、德文、西班牙文、法文和葡萄牙文）。

_**產品發行網路研討會**_&#x200B;在[這裡](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html)觀看2019年6月Release Innovations網路研討會影片。

## 2019年8月 {#august}

2019年8月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

**_每季發行_**

下列功能已於2019年8月16日發行。

## 核心Marketo Engage {#core-marketo-engage}

* **可擴充的網路研討會架構**：運用Marketo全新的現成網路研討會架構（於2019年冬季版本注意事項中推出），將資料從網路研討會提供者無縫傳入Marketo，反之亦然，節省時間。 在這個新架構中，現在可以使用事件和縮放。
* **Smart Campaign API更新**：在我們完成CRUD （建立、讀取、更新、刪除）介面時，管理Smart Campaign生命週期功能。
* **更新電子郵件標頭API變更**：更新電子郵件標頭API不再需要電子郵件附加範本以更新標頭欄位，例如主旨行。

**Account-Based Marketing** ![（顆星）](assets/yellow-star.png)

* **[!DNL LinkedIn]帳戶比對** （先前為測試版）現已正式推出。
* **AccountAI**&#x200B;正在正式重新命名為&#x200B;**帳戶分析**。

<br> 

**_整個季度發行_**

下列功能採用非季度週期，並將在第三日曆季度和2019年第4季度初發佈。

**[!DNL Marketo Sales Connect]** ![（星形）](assets/yellow-star.png)

* **人員頁面配置增強功能：**&#x200B;在新人員頁面配置中，透過清單匯入和大量動作來管理您的人員和群組。

>[!AVAILABILITY]
>
>以星號(![（星號）](assets/yellow-star.png))表示的功能是付費附加元件。 請聯絡您的Marketo代表以瞭解更多資訊。

>[!NOTE]
>
>**TLS 1.0和1.1淘汰**：為符合Adobe的世界級安全性標準，我們將從2019年12月13日起淘汰對傳輸層安全性(TLS) 1.0和1.1的支援。 與Marketo整合的系統若不符合1.2通訊協定，可能會失去對Marketo Engage服務的存取權。
>
>**若要維持您的Marketo Engage存取權，請確定在2019年12月13日之前所有使用者端系統皆符合TLS 1.2規範**。 在[這裡](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)可找到更多詳細資訊。

**_產品發行網路研討會_** [於8月28日1:00PM PT / 4:00PM ET加入我們](https://engage.marketo.com/August_19_Release_Webinar.html)，參加我們產品團隊舉辦的即時網路研討會，並深入瞭解此發行版本包含的功能。
