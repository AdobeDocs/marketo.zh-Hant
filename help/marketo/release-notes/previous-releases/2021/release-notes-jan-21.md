---
description: 發行說明 — 2021年1月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# 發行說明：2021年1月 {#release-notes-jan-21}

』21年1月發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號(![（星號）](assets/yellow-star.png))表示的功能是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_**

下列功能將於2021年1月15日發行。****

## 新一代使用者體驗 {#next-generation-user-experience}

* 支援工作區：Marketo Engage的新一代使用者體驗將Adobe Experience Cloud的外觀和感覺與生產力創新結合，以協助行銷從業人員更快更聰明地工作。 在最新版本中，我們新增了對工作區和分區的完整支援，包括跨工作區共用資料夾的功能。 右側畫布會提供切換開關，讓您可依功能順暢地在舊體驗和新體驗之間轉換，而不會遺失內容。 [深](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) 入了解新一代行銷國家體驗常見問題集。

## 多管道個人化 {#multi-channel-personalization}

* **[Adobe Experience Cloud受眾同步階段3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:現有的Adobe Experience Cloud(AEC)受眾同步功能現在可支援從Marketo Engage到其他AEC應用程式的持續雙向B2B受眾同步，包括Adobe Experience Platform(AEP)產品，例如即時客戶資料平台和Adobe Experience Platform啟動。隨著銷售機會新增並移除至您的受眾區段，Marketo Engage會自動在連線的AEC應用程式中同步更新的受眾。 在AEC技術堆疊中，善用Adobe的多管道協調、重新定位、抑制受眾、個人化和報告使用案例。
* **[持續同步至Google、Facebook和LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**:可以在靜態清單上啟用與廣告網路的連續自動同步，隨著清單成員身份的更改而更新廣告網路，而無需用戶干預。
* **[方案成員自定義欄位的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**:我們已擴充方案成員自訂欄位功能，以支援Token架構。行銷人員可將方案成員自訂欄位代號插入電子郵件、登陸頁面、SMS訊息、推播通知和網頁鈎點。 在促銷活動流程動作中使用新代號來變更資料值、建立任務或有趣的時刻。

## 登陸頁面與Forms {#landing-pages-and-forms}

* **表單API**:從非Marketo表單中提取資料時，提取銷售機會資訊或觸發培養活動。非Marketo表單可透過REST API與Marketo Engage整合。 新的API提供透過所有相關功能模擬Marketo Engage表單提交的功能。
* **登陸頁面API**:透過新的登錄頁面預覽API，簡化整合式應用程式中的編輯和翻譯工作流程。協力廠商現在可以呈現完全個人化的登錄頁面預覽，而不需登入Marketo Engage。  「登錄頁面預覽API」可在協力廠商整合式應用程式中，啟用端對端編輯和本地化工作流程。

## 電子郵件行銷 {#email-marketing}

* **[自訂物件擷取限制已增加](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**:電子郵件速度指令碼的開發人員可以透過自助式覆寫，將自訂物件數量快速增加至100個。行銷人員可存取大量第一層與第二層自訂物件，借此提高智慧型行銷活動的效益。

## Salesforce CRM整合 {#salesforce-crm-integration}

* [Salesforce CRM驗證](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md):OAuth 2.0通訊協定可用於同步Marketo Engage與Salesforce CRM之間的作業。對於新訂閱者，預設會啟用此選項。 目前的訂閱者可聯絡Marketo支援以要求此功能。
* [Salesforce CRM同步控制面板](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md):管理員可以從控制面板快速檢閱Salesforce CRM同步狀態。同步效能報表時間範圍已從2小時增加為5天。
* **中繼資料匯出**:增強以支援機會對象屬性、命名帳戶、程式成員的標準欄位和自定義欄位。

## 管理 {#administration}

* **更新「我的帳戶」頁面**:在「我的帳戶」(My Account)頁上查看基本訂閱資訊。具有任何訪問級別的用戶可以查看訂閱名稱、資料中心標識符和Munchkin ID。

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

* **[增強測試電子郵件工作流程(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**:透過增強的Sales Insight測試電子郵件工作流程，提高您的銷售團隊的效率。銷售者可以先傳送測試電子郵件至所選的電子郵件地址，再傳送大量電子郵件給最多200個收件者。
* **[電子郵件狀態分析(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**:使用者在傳送電子郵件之前，嘗試傳送電子郵件至無效的電子郵件ID或取消訂閱的電子郵件地址時，會看到警告訊息。 您可以在Sales Insight的電子郵件索引標籤中查看電子郵件傳送狀態。
* **從Account和OpportunityPanels( [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) Salesforce  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) CRM)傳送大量電子郵件**:通過使用新的批量操作功能，提高銷售商工作流的效率，並與整個客戶或商機聯繫人清單接洽。使用帳戶或商機標籤中的新下拉式清單選項（而非與個別連絡人合作），傳送電子郵件或新增連絡人至Marketo Engage促銷活動。 將帳戶聯繫人添加到監視清單，以便在銷售機會變熱時收到通知。
* **[非原生Salesforce CRM整合的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**:具有自訂Salesforce CRM整合的GA訂閱可安裝Sales Insight套件，並協助銷售團隊排定最有希望的銷售機會，並與其互動。
* **[最佳增強功能](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**:透過電子郵件傳送或新增至Marketo Engage促銷活動，從「最佳下注」標籤快速聯絡熱線客。在Marketo Engage中檢視銷售機會，或將其新增至您的觀看清單。 在「最佳下注」標籤上執行大量動作和排序選項可節省時間並提高銷售團隊的效率。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **電子郵件連線限制(BETA)**:使用Sales Connect的Email Connection Throttling提高電子郵件傳遞能力並擴展您的1:1銷售通信。我們的全新限制技術可自動管理電子郵件傳送時間，為Exchange和Gmail使用者建立順暢的體驗。 減少或消除第三方大量電子郵件傳送應用程式的使用。
* **電子郵件連線跳出追蹤**:透過新的電子郵件退信報表，深入了解銷售機會品質和電子郵件範本效能。Exchange和Gmail使用者可能會選擇收到退信通知，這些通知會統計至即時摘要、電子郵件資料夾、範本分析和Campaign Analytics。
* **設定檔頁面設定**:在新的設定檔頁面中輕鬆管理使用者偏好設定。變更密碼、編輯地理位置和語言設定，以及集中檢閱整合狀態。
* **範本管理**:使用新的拖放功能將銷售電子郵件範本組織為不同類別，以確保快速存取相關範本並縮短搜尋時間。
* **Sales Connect用戶體驗更新**:通過調整列大小和重新排序列來自定義Sales Connect網格佈局。系統會自動儲存您的檢視偏好設定。

**_公告與淘汰_**

* 在2021年1月15日之前，所有使用者必須升級至Sales Insight **的最新版本。**&#x200B;如果您尚未完成升級，則在登錄到應用程式時，系統將提示您完成升級。 按照本指南](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)中的說明[操作。 更新版本包含已識別安全漏洞的修補程式。 修補程式最初於2016年4月6日發行。 注意：**版本1.4363或更高版本**&#x200B;不需要執行升級。
* 2021年5月&#x200B;**版本將淘汰表單1.0服務。** Forms 1.0服務將完全淘汰，導致剩餘任何仍在使用的Forms 1.0資產功能遺失。 此外，通過不受支援的方法（如將表單POST寫程式到leadCapture/save和leadCapture/save2端點）提交的表單將被拒絕。 如需詳細資訊和修正，請參閱[我們在Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631)中的文章。
* 2021年，Marketo Engage將變更登錄頁面、表單以及影像和檔案資產的URL結構。 針對現有Marketo Engage訂閱，我們將於2021年4月1日開始逐步推出。 有關推出時間表的更多詳細資料將於2021年3月發行。 如需每個受影響資產類型將如何變更的詳細資訊，請參閱行銷國家](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632)中的文章[。

**_產品發行網路研討會_**

想要進一步了解這些功能和增強功能嗎？ 請務必[立即註冊](https://engage.marketo.com/January_21_Release_Webinar_Registration.html)，於1月21日下午1:00 PT /下午4:00 ET加入我們，與我們的產品團隊一起參加線上講座，深入探討這些創新。
