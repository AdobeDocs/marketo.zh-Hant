---
description: 發行說明 — 2021年1月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 0%

---

# 發行說明： 2021年1月 {#release-notes-jan-21}

2021年1月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![（星號）](assets/yellow-star.png))表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將於&#x200B;**2021年1月15日**&#x200B;發行。

## 新一代的使用者體驗 {#next-generation-user-experience}

* 對工作區的支援：Marketo Engage的新一代使用者體驗將Adobe Experience Cloud的外觀與感覺與生產力創新結合在一起，以協助行銷人員更快速、更聰明地工作。 在最新版本中，我們新增對工作區和分割區的完整支援，包括跨工作區共用資料夾的功能。 右側畫布提供切換開關，可讓您為每個功能在舊體驗和新體驗之間無縫轉換，而不會失去內容。 [進一步瞭解](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124)，瞭解有關Marketing Nation的新一代體驗常見問題。

## 多管道Personalization {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync階段3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：現有的Adobe Experience Cloud (AEC) Audience Sync功能現在支援從Marketo Engage到其他AEC應用程式的連續、雙向B2B對象同步，包括Adobe Experience Platform (AEP)產品，例如Real-time Customer Data Platform和Adobe Experience Platform Activation。  當銷售機會新增至您的對象區段並移除時，Marketo Engage會自動在連線的AEC應用程式中同步更新的對象。 善用它，在AEC技術棧疊中善用Adobe的多頻道協調、重新鎖定目標、對象抑制、個人化和報告使用案例。
* **[持續將對象同步到Google、 [!DNL Facebook]和 [!DNL LinkedIn]](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**：可以在靜態清單上啟用與廣告網路的持續自動同步，將廣告網路更新為清單成員資格變更，而不需要使用者介入。
* **[程式成員自訂欄位的權杖](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**：我們已擴充程式成員自訂欄位功能，以支援權杖架構。 行銷人員可以將方案成員自訂欄位權杖插入電子郵件、登陸頁面、SMS訊息、推播通知和Webhook。 在行銷活動流程動作中使用新權杖來變更資料值、建立任務或有趣的時刻。

## 登陸頁面和Forms {#landing-pages-and-forms}

* **表單API**：從非Marketo表單提取資料時，提取銷售機會資訊或觸發Nurture行銷活動。 非Marketo表單可透過REST API與Marketo Engage整合。 新API能夠使用所有關聯功能模擬Marketo Engage表單提交。
* **登陸頁面API**：透過新的登陸頁面預覽API，簡化整合應用程式中的編輯和翻譯工作流程。 協力廠商現在無需登入Marketo Engage，即可呈現完整個人化的登入頁面預覽。  登陸頁面預覽API可在協力廠商整合的應用程式中啟用端對端編輯和本地化工作流程。

## 電子郵件行銷 {#email-marketing}

* **[自訂物件擷取限制增加](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**： Email Velocity指令碼開發人員可透過自助式覆寫，快速將自訂物件數量增加到100個。 行銷人員可存取大量第一級和第二級自訂物件，以提高Smart Campaigns的成效。

## [!DNL Salesforce] CRM整合 {#salesforce-crm-integration}

* [[!DNL Salesforce] CRM驗證](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md)： OAuth 2.0通訊協定可用於Marketo Engage與[!DNL Salesforce] CRM之間的同步作業。 新訂閱者預設會啟用此選項。 目前的訂閱者可聯絡Marketo支援以要求此功能。
* [[!DNL Salesforce] CRM同步儀表板](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md)：管理員可以從儀表板快速檢閱[!DNL Salesforce] CRM同步處理狀態。 同步效能報表時間跨度已從2小時增加到5天。
* **中繼資料匯出**：增強以支援機會物件屬性、具名帳戶、方案成員的標準和自訂欄位。

## 管理 {#administration}

* **已更新我的帳戶頁面**：檢閱[我的帳戶]頁面上的基本訂閱資訊。 具有任何存取層級的使用者可以檢視訂閱名稱、資料中心識別碼和[!DNL Munchkin]識別碼。

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[增強測試電子郵件工作流程([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**：透過增強的[!DNL Sales Insight]測試電子郵件工作流程提高您的銷售團隊效率。 銷售者可以先傳送測試電子郵件給選定的電子郵件地址，再傳送大量電子郵件給最多200位收件者。
* **[電子郵件狀態([!DNL Salesforce] CRM)的深入分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**：使用者在傳送電子郵件之前，嘗試傳送電子郵件至無效的電子郵件ID或取消訂閱的電子郵件地址，就會看到警告訊息。  可以在[!DNL Sales Insight]的電子郵件標籤中檢閱電子郵件傳遞狀態。
* **從[帳戶](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout)和[商機](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout)面板([!DNL Salesforce] CRM)**&#x200B;傳送大量電子郵件：使用新的大量動作功能，改善賣家工作流程的效率，並與整個帳戶或商機連絡人清單互動。 透過在帳戶或機會標籤中使用新的下拉式清單選項（而不是與個別聯絡人合作），傳送電子郵件或新增聯絡人至Marketo Engage行銷活動。 將帳戶連絡人新增至監看清單，以便在潛在客戶成為熱門時收到通知。
* **[[!DNL Sales Insight] 針對非原生 [!DNL Salesforce] CRM整合](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**： GA訂閱搭配自訂Salesforce CRM整合，可以安裝[!DNL Sales Insight]套件，並幫助銷售團隊排定優先順序，並與最有希望的潛在客戶和商機互動。
* **[最佳銷售機會增強功能](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**：透過電子郵件傳送或新增至Marketo Engage促銷活動，快速連絡「最佳銷售機會」標籤的熱門銷售機會。 在Marketo Engage中檢視銷售機會，或將其新增至您的關注清單。 [!UICONTROL Best Bets]標籤上的大量動作和排序選項可節省時間並改善銷售團隊的效率。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **電子郵件連線節流(BETA)**：改善您的電子郵件傳遞能力，並針對[!DNL Sales Connect]調整電子郵件連線節流，以調整1:1銷售通訊。 我們新的節流技術會自動管理電子郵件傳送時間，為[!DNL Exchange]和Gmail使用者建立順暢的體驗。 減少或避免使用協力廠商大量電子郵件傳送應用程式。
* **電子郵件連線跳出追蹤**：透過新的電子郵件跳出報告，讓insight瞭解潛在客戶品質和電子郵件範本效能。 [!DNL Exchange]和Gmail使用者可以選擇接收將彙總至即時摘要、電子郵件資料夾、範本分析和行銷活動分析的退回通知。
* **設定檔頁面組態**：在新設定檔頁面中輕鬆管理使用者偏好設定。 在一個位置變更密碼、編輯地理位置和語言設定，以及檢閱整合狀態。
* **範本管理**：使用新的拖放功能，將銷售電子郵件範本組織成不同類別，以確保能夠快速存取相關範本，並減少搜尋時間。
* **[!DNL Sales Connect]使用者體驗更新**：透過調整欄大小並重新排序來自訂[!DNL Sales Connect]格線版面配置。 您的檢視偏好設定會自動儲存。

**_公告與棄用_**

* 所有使用者必須在2021年1月15日&#x200B;**之前升級至最新版本的Sales Insight**。 如果您尚未完成升級，系統會在您登入應用程式時，提示您完成升級。 請依照本指南](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)中的指示[操作。 更新版本包含已識別安全性弱點的修補程式。 此修補程式最初於2016年4月6日發行。 注意： **1.4363版或以上版本**&#x200B;不需要執行升級。
* Form 1.0服務的棄用將在&#x200B;**2021年5月**&#x200B;發行版本中生效。 Forms 1.0服務將完全淘汰，導致任何仍在使用的Forms 1.0資產失去功能。 此外，透過不支援的方法（例如程式化表單POST至leadCapture/save和leadCapture/save2端點）提交的表單將會遭到拒絕。 如需詳細資訊與補救，請參閱[我們在Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631)的貼文。
* 2021年，Marketo Engage將變更登陸頁面、表單及影像和檔案資產的URL結構。 對於現有的Marketo Engage訂閱，我們將於2021年4月1日開始逐步推出。 有關轉出時間表的更多詳細資訊將於2021年3月發佈。 如需每個受影響資產型別將如何變更的詳細資訊，請參閱[我們在Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632)的貼文。

**_產品發行網路研討會_**

想要進一步瞭解這些功能和增強功能？ 請務必[立即註冊](https://engage.marketo.com/January_21_Release_Webinar_Registration.html)，於1月21日下午1:00 PT / 4:00 PM ET加入我們，與我們的產品團隊一起參加即時網路研討會，以深入瞭解這些創新。
