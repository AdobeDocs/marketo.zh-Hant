---
unique-page-id: 11370952
description: 發行說明- 16年春季版-Marketo文檔——產品文檔
title: 發行說明- 16年春季版
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# 發行說明：彈簧&#39;16 {#release-notes-spring}

Spring &#39;16版本包含下列功能。 請按一下標題連結，以檢視每個功能的詳細文章。

## [電子郵件見解](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

「電子郵件洞察」是全新的歷史資料匯總電子郵件分析體驗— 作為Project Orion的一部分，重新設計了端對端，提供快如閃電的效能。 它提供全新的使用者介面設計，最佳化以符合電子郵件行銷人員的需求和工作流程。

>[!NOTE]
>
>我們將從6月3日開始，分批向客戶推出「電子郵件見解」。 我們的目標是在未來幾個月內完成這項工作。 啟用後，我們會以電子郵件通知您。

![](assets/two.png)

## [電子郵件範本選擇器](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

使用我們新的入門範本建立精美的電子郵件！ 此外，還可從範本的即時縮圖中快速找到範本。

>[!NOTE]
>
>電子郵件編輯器2.0（含範本選擇器）將於6月3日起逐步推出。 我們將於6月30日前完成推出。 與「電子郵件分析」不同，當您有存取權時，不會通知您。 若要瞭解您是否這麼做，請依照[本文](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md)中的步驟進行。

![](assets/5-29-home-starter-templates.png)

## [電子郵件編輯——重新想像](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

沒錯，全新的電子郵件編輯！ 使用輕量型拖放功能來新增及重新排序內容。 新元素，包括影像、視訊、變數和模組，一定能增強您的編輯體驗。 此外，還可檢視更新的程式碼編輯器、預覽器和預先標題支援。

![](assets/17a-29-modules-next.png)

## [行動應用程式內訊息](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

直接在Marketo為您的應用程式建立令人驚艷的應用程式內訊息。 精確定義應該由誰來檢視，以及何時使用應用程式內訊息程式。 使用程式儀表板輕鬆監控其效能。

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [無草稿片段](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md) {#no-draft-snippets}

每次更新程式碼片段時，您都必須重新核准一切的日子已經一去不復返了！ 使用「非草稿」，所有使用程式碼片段的電子郵件和登陸頁面都會取得程式碼片段更新並維持其先前狀態。 每次您核准程式碼片段時，您都可以選擇執行「無草稿」並更新所有內容，或建立草稿。 由您決定！ 「非草稿」將可供所有客戶使用，並由「管理」中的新權限控制。

![](assets/image2016-5-16-15-3a41-3a17.png)

## [著陸頁面、著陸頁面範本和表單API](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

MarketoREST API現在支援控制Marketo登陸頁面、登陸頁面範本和表單。 使用者現在可以直接透過MarketoREST API建立、更新內容、核准和刪除這些資產。

## [API存取的IP允許清單](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

與Marketo使用者登入的IP允許清單功能類似，Marketo管理員現在可以設定可存取MarketoSOAP和REST API的IP位址允許清單，從而封鎖來自非授權IP位址的存取。 這為您的Marketo實例提供了額外的安全層，並確保API存取只能從您組織的網路進行。 有關如何設定此設定的詳細資訊，請參閱[Marketo文檔站點](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md)。

## [全新高速Microsoft Dynamics Sync連接器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

新的高速動態連接器建立在Orion體系結構之上，在初始同步時速度提高了20倍，在增量同步時速度提高了5倍。 所有新客戶將在發行日期上線至此連接器，我們將在夏季發行時間範圍內逐步向現有客戶推出。

**重新整理新欄位的資料**:現在，您可以在任何時間點啟用新的同步欄位，該欄位的所有資料值都將從Dynamics CRM重新整理至Marketo。不必再擔心在初始設定期間必須選取所有欄位。 如果您停用現有的同步欄位並稍後重新啟用，該欄位的所有資料值都會從Dynamics CRM重新整理到Marketo。

**將銷售線索作為聯繫人同步**:「將銷售線索同步到Microsoft流」操作有一個新選項，可以作為銷售線索或聯繫人進行同步。

![](assets/image2016-5-19-8-3a59-3a9.png)

**同步錯誤管理標籤**:瀏覽、搜尋或匯出無法與操作、方向、錯誤碼和錯誤訊息等詳細資訊同步的潛在客源（及其他物件）。

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**:Connector已完全認證Dynamics 2016線上和內部部署版本。

**外掛程式更新現在已記錄在案：請** 參閱外 [掛程式更新檔案文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)。

## [友好實例名稱](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

如今，很難區分Marketo例項，例如沙盒和生產例項。 此功能可讓您瞭解目前正在處理的例項。

![](assets/image2016-5-16-15-3a57-3a14.png)

## [訂閱的限時存取權](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

今天，使用者將獲邀無限期訂閱Marketo。 此功能可讓管理員邀請使用者在限定的期間內訂閱，例如2週或1個月。

![](assets/image2016-5-16-15-3a59-3a52.png)

## [自訂物件格線](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

現在，您可以檢視所有已發佈自訂物件的記錄和欄位數。

![](assets/custom-objects-grid.png)

## 自訂活動{#custom-activities}

Marketo管理員現在可以透過「Marketo自訂活動定義」建模器來定義及管理其自訂活動類型。 與「Marketo自訂物件建模器」類似（並與之搭配），管理員現在可以擴充資料模型，以符合其確切的業務需求。 有關如何使用此功能的詳細資訊，請參閱[Marketo文檔站點](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md)。
