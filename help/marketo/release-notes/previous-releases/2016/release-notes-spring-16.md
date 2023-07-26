---
unique-page-id: 11370952
description: 發行說明–2016年春季 — Marketo檔案 — 產品檔案
title: 發行說明 — 2016年春季
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# 發行說明： 2016年春季 {#release-notes-spring}

以下功能包含在2016年春季發行版本中。 請按一下標題連結以檢視每個功能的詳細文章。

## [電子郵件深入分析](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

電子郵件深入解析是全新的歷史彙總資料電子郵件分析體驗 — 重新設計端對端，作為Project Orion的一部分提供超快效能。 其特色是全新使用者介面設計，已最佳化以符合電子郵件行銷人員的需求和工作流程。

>[!NOTE]
>
>自6月3日起，我們將分批向客戶推出電子郵件深入分析。 我們的目標是在未來幾個月內完成這項工作。 我們會在您啟用時透過電子郵件通知您。

![](assets/two.png)

## [電子郵件範本選取器](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

使用我們新的入門範本建立精美的電子郵件！ 此外，從範本的即時縮圖快速找到您的範本。

>[!NOTE]
>
>電子郵件編輯器2.0 （含範本選擇器）將於6月3日起逐步推出。 我們將在6月30日前完成推出。 不同於電子郵件分析，當您具有存取權時，您不會收到通知。 若要檢視您是否這樣做，請依照中的步驟操作 [本文](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [電子郵件編輯 — 重新想像](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

沒錯，全新的電子郵件編輯器！ 使用輕量型的拖放功能來新增及重新排序內容。 新元素（包括影像、影片、變數和模組）必定能增強您的編輯體驗。 另請檢視更新的程式碼編輯器、預覽器和預覽器支援。

![](assets/17a-29-modules-next.png)

## [行動應用程式內訊息](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

直接在Marketo中為您的應用程式建立令人驚歎的應用程式內訊息。 精確地定義應該看到的人以及使用應用程式內訊息程式的時機。 使用程式儀表板輕鬆監控其效能。

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [無草稿程式碼片段](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md) {#no-draft-snippets}

您每次更新程式碼片段時必須重新核准所有專案的日子已一去不復返！ 透過無草稿，所有使用程式碼片段的電子郵件和登陸頁面都會收到程式碼片段更新，並保持其先前的狀態。 每次核准程式碼片段時，您都可以選擇執行無草稿並更新所有專案，或建立草稿。 由您決定！ 無草稿可供所有客戶使用，並由Admin中的新許可權控制。

![](assets/image2016-5-16-15-3a41-3a17.png)

## [登陸頁面、登陸頁面範本及表單API](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Marketo REST API現在支援控制Marketo登陸頁面、登陸頁面範本和表單。 使用者現在可以直接透過Marketo REST API建立、更新內容、核准和刪除這些資產。

## [API存取的IP允許清單](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

與Marketo使用者登入的IP允許清單功能類似，Marketo管理員現在可以設定IP位址允許清單，以存取Marketo SOAP和REST API，進而封鎖來自未授權IP位址的存取。 這為您的Marketo執行個體提供額外的安全層，並確保API存取只能從您組織的網路中進行。 有關如何進行此設定的詳細資訊，請參閱 [Marketo檔案網站](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [新的高速Microsoft Dynamics同步聯結器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

全新的高速動態聯結器建置在Orion架構之上，提供高達20倍的初始同步速度，以及高達5倍的增量同步速度。 所有新客戶將在發行日期加入此聯結器，我們將在夏季發行時間範圍內逐步向現有客戶推出。

**重新整理新欄位的資料**：您現在隨時可以啟用新的同步欄位，該欄位的所有資料值將會從Dynamics CRM重新整理至Marketo。 不用擔心在初始設定期間必須選取所有欄位。 如果您停用現有的同步欄位並在稍後重新啟用，該欄位的所有資料值將會從Dynamics CRM重新整理至Marketo。

**將銷售機會同步為連絡人**：同步至Microsoft的銷售機會流程動作有一個新選項，可讓您以銷售機會或連絡人的身分進行同步。

![](assets/image2016-5-19-8-3a59-3a9.png)

**同步錯誤管理標籤**：瀏覽、搜尋或匯出無法與操作、方向、錯誤代碼和錯誤訊息等詳細資訊同步化的潛在客戶（和其他物件）。

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**：聯結器已針對Dynamics 2016線上和內部部署版本通過完整認證。

**此外掛程式更新現在已記錄下來：** 請參閱 [外掛程式更新檔案文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [好記的執行個體名稱](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

現今，很難區分Marketo執行個體，例如沙箱和生產執行個體。 此功能可讓您知道您目前正在處理哪些執行個體。

![](assets/image2016-5-16-15-3a57-3a14.png)

## [訂閱的有限時間存取](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

現在，使用者受邀無限期訂閱Marketo。 此功能可讓管理員在有限的時間內邀請使用者訂閱，例如2週或1個月。

![](assets/image2016-5-16-15-3a59-3a52.png)

## [自訂物件格線](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

現在，您可以檢視所有已發佈自訂物件的記錄數和欄位數。

![](assets/custom-objects-grid.png)

## 自訂活動 {#custom-activities}

Marketo管理員現在可以透過Marketo自訂活動定義模組化工具來定義和管理其自訂活動型別。 類似（並結合） Marketo自訂物件建模工具，管理員現在可以擴充資料模型，以符合其確切的業務需求。 欲知如何使用此功能的詳情，請參閱 [Marketo檔案網站](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
