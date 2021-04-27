---
description: 發行說明- 2021年1月-Marketo文檔——產品文檔
title: 發行說明- 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
translation-type: tm+mt
source-git-commit: 7566581555eb95564b9f69884190dd987e123dbe
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# 發行說明：2021年1月{#release-notes-jan-21}

1月21日發行包含下列功能。 查看您的Marketo版功能是否可用。

>[!AVAILABILITY]
>
>以星號(![(star)](assets/star-yellow.svg))表示的功能是付費附加元件。 請連絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

**2021年1月15日**&#x200B;將發佈下列功能。

## 新一代用戶體驗{#next-generation-user-experience}

* 支援工作區：Marketo Engage新一代的使用者體驗將Adobe Experience Cloud的外觀和感覺與生產力創新結合在一起，協助行銷從業人員更快更聰明地工作。 在最新版本中，我們新增了對工作區和分區的完整支援，包括跨工作區共用資料夾的功能。 右側畫布提供切換切換切換功能，讓您在每個功能之間順暢地轉換舊體驗和新體驗，而不會遺失內容。 [進一](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) 步瞭解Marketing Nation的新一代體驗常見問答集。

## 多通道個人化{#multi-channel-personalization}

* **[Adobe Experience Cloud觀眾同步階段3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:現有的Adobe Experience Cloud(AEC)觀眾同步功能現在支援從Marketo Engage到其他AEC應用程式的連續、雙向B2B觀眾同步，包括Adobe Experience Platform(AEP)方案，例如即時客戶資料平台和Adobe Experience Platform啟動。當客源新增並移除至您的受眾細分時，Marketo Engage將自動同步您所連線之AEC應用程式中更新的受眾。 運用它，在AEC技術團隊中運用Adobe的多通道協調、重新定位目標、抑制受眾、個人化和報告使用案例。
* **[Continuous Audience Sync to Google、Facebook和LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**:可以在靜態清單上啟用與廣告網路的連續自動同步，隨著清單成員資格的改變更新廣告網路而無需用戶干預。
* **[方案成員自訂欄位的代號](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**:我們擴充了方案會員的自訂欄位功能，以支援Token架構。行銷人員可將方案會員的自訂欄位Token插入電子郵件、登陸頁面、SMS訊息、推播通知和網頁勾點。 在促銷活動流程動作中使用新的Token來變更資料值、建立工作或有趣的時刻。

## 著陸頁面與Forms{#landing-pages-and-forms}

* **表單API**:從非Marketo表單提取資料時，可獲取銷售線索資訊或觸發培育宣傳活動。非Marketo表單可透過REST API與Marketo Engage整合。 新API提供模擬Marketo Engage表單提交與所有相關功能的能力。
* **著陸頁面API**:使用全新的著陸頁面預覽API，簡化整合式應用程式的編輯和翻譯工作流程。協力廠商現在可以轉換完全個人化的登陸頁面預覽，毋需登入Marketo Engage。  「著陸頁面預覽API」可在協力廠商整合應用程式中啟用端對端編輯和本地化工作流程。

## 電子郵件行銷{#email-marketing}

* **[自訂物件擷取限制已增加](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**:電子郵件速度指令碼開發人員可以透過自助覆寫功能，將自訂物件數量快速增加到100個。行銷人員可存取大量的第一層與第二層自訂物件，以提高「智慧型促銷活動」的效率。

## Salesforce CRM整合{#salesforce-crm-integration}

* [Salesforce CRM驗證](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md):OAuth 2.0通訊協定可用於同步Marketo Engage與Salesforce CRM之間的作業。對於新訂閱者，預設會啟用此選項。 目前的訂閱者可聯絡Marketo支援部門以要求這項功能。
* [Salesforce CRM同步儀表板](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md):管理員可從儀表板快速檢閱Salesforce CRM同步狀態。同步效能報表的時間間隔已從2小時增加為5天。
* **中繼資料匯出**:增強功能可支援機會物件屬性、命名帳戶、方案會員的標準欄位和自訂欄位。

## 管理{#administration}

* **已更新我的帳戶頁面**:在「My Account（我的帳戶）」頁面上檢閱基本訂閱資訊。具有任何存取等級的使用者可以檢視訂閱名稱、資料中心識別碼和Munchkin ID。

**_整季發行_**

以下功能是非季度週期，將於未來數月內發佈。

## 銷售分析{#sales-insight}

![（星號）](assets/star-yellow.svg)

* **[增強的測試電子郵件工作流程(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**:透過增強的Sales Insight測試電子郵件工作流程，提高銷售團隊的效率。銷售者可先將測試電子郵件傳送至所選的電子郵件地址，再將大量電子郵件傳送給最多200位收件者。
* **[電子郵件狀態分析(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**:當使用者嘗試在傳送電子郵件之前，先傳送電子郵件至無效的電子郵件ID或未訂閱的電子郵件地址時，會看到警告訊息。 您可以在Sales Insight的電子郵件標籤中查看電子郵件傳送狀態。
* **從AccountPanels和 [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) OpportunityPanels(Salesforce CRM) [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) 傳送大量電子郵件**:使用全新的大量動作功能來改善賣方工作流程並與整個帳戶或機會聯絡人清單互動。使用帳戶或業務機會標籤中的新下拉式選項，而非使用個別聯絡人，以傳送電子郵件或新增聯絡人至Marketo Engage促銷活動。 將帳戶聯絡人新增至監看清單，以便在潛在客戶變熱時收到通知。
* **[針對非原生Salesforce CRM整合的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**:具有自訂Salesforce CRM整合的GA訂閱可安裝Sales Insight套件，並協助銷售團隊排定最有希望的潛在客戶和機會的優先順序，並與之互動。
* **[最佳增強功能](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**:透過電子郵件傳送或新增至Marketo Engage促銷活動，從「最佳下注」標籤快速聯絡熱門客源。在Marketo Engage中檢視銷售線索，或將其新增至您的監視清單。 「最佳下注」標籤上的大量動作和排序選項可節省時間並改善銷售團隊的效率。

## 銷售連接{#sales-connect}

![（星號）](assets/star-yellow.svg)

* **電子郵件連線限制(BETA)**:使用Sales Connect的電子郵件連線限制功能，改善您的電子郵件傳遞能力並擴大您的一對一銷售通訊。我們的全新調節技術會自動管理電子郵件傳送時間，為Exchange和Gmail使用者建立順暢的體驗。 減少或免除使用協力廠商大量電子郵件傳送應用程式。
* **電子郵件連線彈回數追蹤**:透過新的電子郵件反彈報表，深入瞭解銷售機會品質和電子郵件範本效能。Exchange和Gmail使用者可能會選擇收到反彈通知，這些通知會統計至即時動態消息、電子郵件資料夾、範本分析和促銷活動分析。
* **描述檔頁面設定**:在新的設定檔頁面中輕鬆管理使用者偏好設定。變更密碼、編輯地理位置和語言設定，並集中審核整合狀態。
* **範本管理**:使用全新的拖放功能，將銷售電子郵件範本組織成類別，以確保快速存取相關範本並縮短搜尋時間。
* **Sales Connect使用者體驗更新**:調整欄的大小並重新排序，以自訂Sales Connect格線版面。您的檢視偏好設定會自動儲存。

**_公告與淘汰_**

* 所有使用者必須在2021年1月15日前升級至最新版的Sales Insight **。**&#x200B;如果您尚未完成升級，當您登入應用程式時，將會提示您進行升級。 請遵循本指南](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)中的說明。 [更新版本包含已識別安全性弱點的修補程式。 修補程式最初於2016年4月6日發行。 注意：**1.4363或更新版本**&#x200B;不需要執行升級。
* 取消表單1.0服務將於2021年5月&#x200B;**發行中生效。** Forms1.0服務將完全停用，導致任何仍在使用的Forms1.0資產的功能喪失。 此外，透過不支援的方法（例如程式化表單POST）提交至leadCapture/save和leadCapture/save2端點的表單，也會被拒絕。 如需詳細資訊和修正，請參閱[我們在Marketing Nation中的貼文](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631)。
* 在2021年，Marketo Engage將變更著陸頁面、表單、影像和檔案資產的URL結構。 就現有Marketo Engage訂閱而言，我們將於2021年4月1日開始逐步推出。 推出時間表的更多詳細資訊將於2021年3月發佈。 如需每個受影響資產類型將如何變更的詳細資訊，請參閱「行銷國家」中的[貼文。](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632)

**_產品發行網路研討會_**

想要進一步瞭解這些功能和增強功能嗎？ 請記得[立即註冊](https://engage.marketo.com/January_21_Release_Webinar_Registration.html)，在1月21日下午1:00 PT / 4:00 PM ET加入我們，與我們的產品團隊進行即時網路研討會，深入探討這些創新。
