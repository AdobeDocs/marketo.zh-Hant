---
description: 發行說明 — 2021年5月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2021年5月
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# 發行說明： 2021年5月 {#release-notes-may-21}

2021年5月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將會發行於 **2021年5月7日**.

## 帳戶型體驗 {#Account-based-eaperiences}

* **帳戶智慧清單（一般可用性）** ![](assets/yellow-star.png)：使用所需的帳戶和人員屬性，以動態方式識別並限定帳戶，以便在跨頻道行銷活動中定位，並及時傳送警報給銷售人員，以便更快完成交易。 這項新功能可讓帳戶式行銷策略實現強大的自動化功能。 帳戶智慧清單適用於擁有新一代使用者體驗之Target帳戶管理的客戶。

## 新一代的使用者體驗 {#next-generation-user-experience}

透過全域搜尋預覽，行銷人員可快速檢視共用資產存在於其例項中的位置。 瀏覽器標籤會顯示可改善行銷活動或Design Studio中導覽的位置。 其他樹狀結構和全域搜尋篩選器有助於縮小您的搜尋條件。 樹狀結構中的拖放功能已恢復，讓您在主要應用程式區域中快速且有效率地行動資料夾和資產。 最新更新的圖示(符合Adobe的協助工具標準)和狀態徽章可讓行銷人員在樹狀結構中快速輕鬆地區分資料夾和資產，並識別計畫和資產的狀態。

## 體驗自動化 {#experience-automation}

* **執行Campaign流程步驟**：使用Smart Campaigns的全新流程步驟，簡化行銷活動建立工作流程並改善行銷活動績效。 透過新的「執行行銷活動」流程步驟，從任何Smart Campaign呼叫並執行的工作區中重複工作（例如國家/地區程式碼標準化）的集中範本行銷活動，並加以儲存。 連結的行銷活動會以指定的順序執行，並在前進到下一個流程步驟之前確保任務完成。 在一個集中式行銷活動中快速編輯流程，以更新使用它的每個Smart Campaign，簡化資料管理、領導評分和路由工作流程。

## 跨頻道協調 {#cross-channel-orchestration}

* **Forms中的敏感資料欄位**：將資料欄位定義為敏感，並限制這些欄位的表單預填，以防止Protect客戶的個人識別資訊(PII)顯示在Adobe Marketo Engage表單中。 每當訪客檢視登入頁面上的表單時，定義為敏感的欄位都不會顯示任何預先填入的資料。

* **封鎖垃圾郵件表單提交**：Protect您的Adobe Marketo Engage資料庫，防止垃圾郵件資料對銷售人員造成無效警示、觸發行銷活動積壓，以及建立不需要的活動。 新的驗證機制會拒絕無效的表單提交並停止機器人攻擊。 您的資料更乾淨，行銷活動會如預期運作，將傳送不合格銷售線索的風險降至最低。

* **以電子郵件傳送方案核准警告**：防止在對先前核准的方案進行新編輯時傳送錯誤電子郵件。  當行銷人員將變更套用至已核准的電子郵件，但隨後忘記核准最新變更時，警告會充當護欄，並傳送電子郵件給沒有內容、不良內容或舊內容的大型對象。

* **篩選出電子郵件機器人活動**：透過新的電子郵件機器人活動篩選功能，防止意外銷售警報和不正確的電子郵件報告。 識別並篩選出可能與電子郵件機器人相關聯的開啟和點按，檢查導致錯誤觸發器和銷售警報，或不正確報告的連結。

## API增強功能 {#api-enhancements}

大量和潛在客戶API的幾項重要更新，包括大量匯出自訂物件資料的功能、將公司與潛在客戶大量建立關聯的功能、根據主要屬性篩選大量活動擷取的功能，以及建立和更新方案成員資格的功能。

* **巢狀內嵌事件程式**：在Adobe Marketo Engage中，您可以建立、複製或移動其他程式型別下的事件程式。 資產API現在允許此功能。

* **增強型刪除計畫API**：可讓整合式應用程式刪除包含其他資產型別的程式，而不需要使用者從Adobe Marketo Engage手動操作。

* **計畫會籍**：行銷人員可查詢指定不同條件（例如方案成員狀態）之選定方案的所有方案成員記錄。 與外部應用程式、商業智慧工具或Adobe Experience Cloud共用這些資訊，以改進細分並建立更有針對性的參與。

* **大量自訂物件擷取**：大量資料匯出可補充資料分析人員在Adobe Marketo Engage中已經擁有的匯入功能。 現在，他們可以大量擷取儲存在第一級Adobe Marketo Engage自訂物件中的資料，將此資料載入另一個應用程式、Data Warehouse或BI (Business Intelligence)工具，以更深入瞭解Adobe Marketo Engage例項中的資料。  自訂物件大量資料移動是雙向的，可以在方便的時間進行排程。

* **自訂欄位中繼資料API**：設定Adobe Marketo Engage與第三方應用程式的整合，並自動建立自訂欄位，以節省時間。 這項自動化對擁有多個Adobe Marketo Engage執行個體的客戶來說尤其有利，這些客戶現在能夠簡化自訂欄位的建立，以前需要在每個執行個體中手動操作。 簡化自訂欄位的建立，並節省此資源消耗活動的時間。

* **大量活動擷取API**：執行大量擷取時，可控制資料的數量和型別。 篩選掉不必要的資料點，並控制大量擷取活動資料所需的API呼叫數。  例如，選取開啟的電子郵件、造訪網頁，或變更潛在客戶分數，並留下您不想分析的其他值變更。 簡化程式，減少API呼叫和資料清理的數量。

* **銷售機會API**：識別Adobe Marketo Engage中擁有相關聯之AdobeECID (Experience CloudID)的銷售機會。  Adobe Marketo Engage客戶可以從選取的行銷活動建立銷售機會清單，並使用ECID (Experience CloudID)在Adobe Analytics中建立該特定清單的報告。 Adobe Marketo Engage與Adobe Experience Cloud的整合為細分、鎖定目標和報告開啟了無限商機。

* **大量潛在客戶匯入API**：控制大量潛在客戶匯入及其所花費的資源。 此增強功能會在大量潛在客戶匯入程式期間，建立潛在客戶與公司之間的關聯。 如果API呼叫，可提升處理資料的效率並降低使用量。

* **適用於Microsoft Dynamics Online客戶的Web API型整合**：MS Dynamics Web API隨8.0版REST通訊協定引入，並實作OData （開放資料通訊協定） v4。 OData是OASIS (Organization for the Advanced of Structured Information Standards)標準，用於建置和使用RESTful服務以取代豐富的資料。 需要使用此方法與Microsoft Dynamics整合的Adobe Marketo Engage客戶，目前正在從SOAP （簡單物件存取通訊協定）移轉至Web API型連線。

## 行銷資料環境 {#marketing-data-environment}

* **XLSX匯出**：我們已升級整個產品的匯出功能，以支援XLSX來取代XLS。 這表示在產品中目前支援XLS匯出的任何位置，此選項將取代為匯出至XLSX的選項。 此變更將會影響從Adobe Marketo Engage匯出報表及其他資料的所有Excel匯出的檔案名稱。

* **依銷售機會ID搜尋**：快速存取潛在客戶資料庫或靜態清單中依Adobe Marketo Engage潛在客戶ID搜尋的潛在客戶記錄。 在「快速搜尋」視窗中，直接輸入 `[id]` ，則會顯示潛在客戶資訊。 使用者可以快速檢視潛在客戶、公司或商機的詳細資訊。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **與LinkedIn Lead Gen Forms (Beta)整合**：使用Bizible Premium歸因解決方案，深入掌握您的LinkedIn管道支出和ROI。 透過與LinkedIn的Lead Gen Forms的最新整合，Bizible得以深入瞭解在LinkedIn平台內提交的表單。 這些表單填寫會比對您CRM （客戶關係管理）或Adobe Marketo Engage執行個體的銷售機會，因此符合歸因資格，並可根據您的其他行銷活動進行追蹤。

## 公告 {#announcements}

* **Marketo產品檔案切換平台**：我們很高興宣佈，Marketo產品檔案已於5月7日星期五起加入Adobe Experience League。 您仍可使用URL： docs.marketo.com ，如果您有任何已建立書籤的現有文章，系統將會重新導向您。 新平台提供所有產品檔案，並計畫於今年晚些時候推出增強功能。

* **由AdobeIdentity System提供支援的簡化使用者管理和單一登入**：自2021年7月起，新的Adobe Marketo Engage客戶將使用Adobe使用者憑證上線。 目前客戶至整合式身分系統的移轉作業要到2022年年中才會進行，且客戶須另行通知後才能採取行動。 單一登入可讓IT/安全性管理員管理多個Adobe Marketo Engage產品執行個體及其他Experience Cloud解決方案，並透過共用主控台設定SSO （Shared Services組織）。 管理員可以透過通用Admin Console方便地管理使用者群組和使用者權益。

**_產品發行網路研討會_**

[2021年5月Marketo Engage版本網路研討會](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
