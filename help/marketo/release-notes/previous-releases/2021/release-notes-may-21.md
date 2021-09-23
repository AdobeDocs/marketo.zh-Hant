---
description: 發行說明 — 2021年5月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2021年5月
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1481'
ht-degree: 0%

---

# 發行說明：2021年5月 {#release-notes-may-21}

』21年5月發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))表示的功能為付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_**

下列功能將於2021年5月7日發行。****

## 帳戶型體驗 {#Account-based-eaperiences}

* **帳戶智慧清單（正式發行）** ![](assets/yellow-star.png):在跨通路行銷活動中動態識別並限定具有所需帳戶和人員屬性以鎖定的帳戶，並及時傳送警報給銷售人員，以更快完成交易。這項新功能可讓帳戶型行銷策略的強大自動化。 具有Target帳戶管理的客戶可在新一代使用者體驗上使用帳戶智慧清單。

## 新一代使用者體驗 {#next-generation-user-experience}

透過全域搜尋預覽，行銷人員可以快速查看其例項中共用資產的所在位置。 瀏覽器標籤顯示可改善行銷活動或Design Studio中導覽的位置。 其他樹狀結構和全域搜尋篩選器有助於調整您的搜尋條件。 樹狀結構中的拖放功能已恢復，可讓您在主要應用程式區域中快速且有效地移動資料夾和資產。 新更新的圖示(符合Adobe的協助工具標準)和狀態徽章可讓行銷人員在樹狀結構中快速輕鬆地區分資料夾和資產，並識別方案和資產的狀態。

## 體驗自動化 {#experience-automation}

* **執行促銷活動流程步驟**:透過智慧型行銷活動的新流程步驟，簡化行銷活動建立工作流程並改善行銷活動績效。建立並儲存工作區中重複性工作的集中範本促銷活動，例如國家/地區代碼標準化，並透過新的「執行促銷活動」流程步驟，從任何智慧型促銷活動呼叫及執行。 連結的促銷活動將以指定順序執行，並在前進至下一個流程步驟之前確保任務完成。 只需在一個集中式行銷活動中快速編輯流程，以更新每個使用該流程來簡化資料管理、銷售機會評分和傳送工作流程的智慧行銷活動。

## 跨管道協調 {#cross-channel-orchestration}

* **Forms中的敏感資料欄位**:ProtectAdobeMarketo Engage表單中無法顯示客戶的個人識別資訊(PII)，方法是將資料欄位定義為敏感欄位，並限制這些欄位的表單預填。每當訪客在登陸頁面上檢視表單時，定義為敏感的欄位將不會顯示任何預先填入的資料。

* **阻止垃圾郵件表單提交**:Protect您的AdobeMarketo Engage資料庫，其可能會對銷售產生無效警報、觸發促銷活動積壓，以及建立不想要的活動。新的驗證機制會拒絕無效的表單提交，並停止機器人攻擊。 您的資料更乾淨，而您的行銷活動會如預期般運作，將傳送不合格銷售機會至銷售的風險降至最低。

* **電子郵件計畫批准警告**:防止在對先前核准的程式進行新編輯時傳送錯誤的電子郵件。當行銷人員將變更套用至已核准的電子郵件，但之後忘記核准最新變更，並將電子郵件傳送給沒有內容、不良內容或舊內容的大型對象時，此警告可作為防護措施。

* **篩除電子郵件機器人活動**:透過新的電子郵件機器人活動篩選功能，防止非預期的銷售警報和不正確的電子郵件報告。識別並篩除可與電子郵件機器人相關聯的開啟和點按，以檢查導致錯誤觸發器和銷售警報的連結，或錯誤報告。

## API增強功能 {#api-enhancements}

對Bulk和Lead API進行數項重要更新，包括能夠大量匯出自訂物件資料、大量關聯公司與銷售機會、能夠根據主要屬性篩選大量活動擷取，以及能夠建立和更新方案成員資格。

* **巢狀內嵌事件程式**:在「Adobe」Marketo Engage中，您可以建立、複製或移動其他程式類型下的事件程式。資產API現已允許此功能。

* **增強的刪除方案API**:允許整合應用程式刪除包含其他類型資產的程式，而無需用戶從AdobeMarketo Engage手動刪除。

* **方案成員資格**:行銷人員可以查詢指定不同條件（如方案成員狀態）之選定方案的所有方案成員記錄。與外部應用程式、業務智慧工具或Adobe Experience Cloud共用此資訊，以改善細分並建立更具針對性的參與。

* **大量自訂物件擷取**:大量資料匯出補充了資料分析師在AdobeMarketo Engage中已具備的匯入功能。現在，他們可以大量擷取儲存在第一級AdobeMarketo Engage自訂物件中的資料，將此資料載入至其他應用程式、資料倉儲或BI(Business Intelligence)工具，以更深入分析AdobeMarketo Engage例項中的資料。  自訂物件大量資料移動是雙向的，可在方便的時間排程。

* **自訂欄位中繼資料API**:自動建立自訂欄位，同時設定與第三方應用程式的AdobeMarketo Engage整合，以節省時間。此自動化特別讓擁有多個AdobeMarketo Engage例項的客戶受益，這些例項現在能夠簡化建立自訂欄位的流程，而以往每個例項都需要手動操作。 簡化自訂欄位的建立，並節省此資源消耗活動的時間。

* **大量活動擷取API**:在執行大量擷取時，獲得對資料量和類型的控制。篩選掉不必要的資料點，並控制大量擷取活動資料所需的API呼叫數。  例如，選擇開啟的電子郵件、瀏覽網頁或銷售機會分數的變更，並保留您不想分析的其他值變更。 簡化程式，減少API呼叫和資料清除的數量。

* **銷售機會API**:識別AdobeMarketo Engage中與其相關聯的AdobeECID(Experience CloudID)銷售機會。AdobeMarketo Engage客戶可從選取的促銷活動建立銷售機會清單，並使用ECID(Experience CloudID)在Adobe Analytics中建立該特定清單的報表。 AdobeMarketo Engage與Adobe Experience Cloud的整合為區段、鎖定目標和報告提供無限的機會。

* **大量銷售機會匯入API**:控制大量銷售機會匯入及其所需資源。此增強功能會在大量銷售機會匯入程式期間，建立銷售機會與公司之間的關聯。 提高處理資料的效率，並減少API呼叫時的使用。

* **基於Web API的Microsoft Dynamics Online客戶整合**:MS Dynamics Web API隨8.0版REST通訊協定推出，並實作OData（開放資料通訊協定）v4。OData是OASIS（結構化資訊標準提升組織）標準，用於構建和使用RESTful服務來覆蓋豐富的資料。 AdobeMarketo Engage客戶若需使用此方法與Microsoft Dynamics整合，目前正從SOAP（簡單物件存取通訊協定）移轉至Web API型連線。

## 行銷資料環境 {#marketing-data-environment}

* **XLSX匯出**:我們升級了整個產品的匯出功能，以支援XLSX取代XLS。這表示目前支援XLS匯出的產品中任何地方，都會以選項取代此選項，以改用XLSX匯出。 此變更會影響所有Excel匯出之報表和其他資料的檔案名稱，這些資料來自AdobeMarketo Engage。

* **依銷售機會ID搜尋**:按銷售機會資料庫或靜態清單中的AdobeMarketo Engage銷售機會ID快速訪問銷售機會記錄搜索。在「快速查找」窗口中，只需鍵入具有相應編號的`[id]`，然後顯示銷售線索資訊。 用戶可以快速查看銷售機會、公司或銷售機會詳細資訊。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **與LinkedIn Lead Gen Forms（測試版）整合**:透過Bizible premium歸因解決方案，深入掌握您的LinkedIn管道支出和ROI。透過與LinkedIn的Lead Gen Forms的最新整合，Bizible可深入分析LinkedIn平台中已提交的表單。 這些表單填入會與來自您CRM（客戶關係管理）或AdobeMarketo Engage例項的銷售機會相符，因此他們符合歸因資格，並可根據您的其他行銷活動受到追蹤。

## 公告 {#announcements}

* **Marketo產品檔案切換平台**:很高興在此宣佈，自5月7日星期五起，Marketo產品檔案已加入Adobe Experience League。您仍可使用URL:docs.marketo.com，若您有任何已建立書籤的文章，系統會將您重新導向。 所有產品檔案都可在新平台上取得，並預計於今年晚些時候提供增強功能。

* **由Adobe識別系統支援的簡化使用者管理和單一登入**:自2021年7月起，新的AdobeMarketo Engage客戶將使用Adobe使用者認證上線。直到2022年年中，才會將現有客戶移轉至整合身份系統，在進一步通知之前，無需客戶採取任何操作。 單一登入可讓IT/安全管理員管理多個AdobeMarketo Engage產品例項以及其他Experience Cloud解決方案，並透過共同主控台設定SSO（Shared Services組織）。 管理員可透過通用Admin Console，輕鬆管理使用者群組和使用者權益。

**_產品發行網路研討會_**

想要進一步了解這些功能和增強功能嗎？ 請務必[立即註冊](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)，在5月13日上午9:00 PT /中午12:00 ET加入我們，與我們的產品團隊一起舉辦線上講座，以深入探討這些創新。
