---
unique-page-id: 37356893
description: MSI功能總覽 — Marketo檔案 — 產品檔案
title: MSI功能概述
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: bda95da160c5a27a0a460d26c102e6166c1ddea0
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# MSI功能概述 {#msi-feature-overview}

MSI在Salesforce Lightning and Classic中提供下列功能。

>[!NOTE]
>
>為了檢視所有可用的資料，請確保在使用Windows時將瀏覽器縮放比例設定為不超過125%，在Mac作業系統上則設定為150%。

## Visualforce面板 {#visualforce-panel}

MSI Visualforce面板包含下列功能：

* 索引標籤

   * [見解控制面板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * 有趣的時刻
   * 網頁活動
   * 電子郵件
   * 分數

* 動作

   * 新增至Marketo Campaign
   * 傳送Marketo電子郵件
   * 新增/移除監看清單

* 星星和火焰

## 潛在客戶配置 {#lead-layout}

Visualforce頁面：

* 銷售機會 — 包含按一下「前往完整清單」的超選項，您將會被送到Salesforce中的新索引標籤，其中MSI面板將顯示在全頁版面配置中
* 潛在客戶完整清單 — 不包含「前往完整清單」選項
* 潛在客戶行動 — 顯示在Salesforce行動應用程式中
* 潛在客戶聯絡人Bridge — 顯示您已新增至MSI聯絡人ID欄位之聯絡人的MSI面板

欄位：

* 上一個有趣的時刻
* 上一個有趣的時刻日期
* 上一個有趣時刻說明
* Source最後有趣的時刻
* 上一個有趣的時刻型別
* 最後一個Marketo活動（依銷售分列）
* 銷售人員的最後一次Marketo參與
* 相對分數
* 相對分數值
* 急迫性
* 緊急值
* 在Marketo中檢視 — 按一下此欄位可開啟Marketo中潛在客戶的不可編輯檢視。 包括：銷售機會資訊、公司資訊、SFDC銷售機會資訊、SFDC自訂欄位、活動記錄
* MSI聯絡人ID — 將Salesforce聯絡人新增至此欄位，並在潛在客戶配置中包含「潛在客戶聯絡人Bridge」面板，以檢視聯絡人的MSI面板

## 連絡人配置 {#contact-layout}

Visualforce頁面：

* 連絡人 — 包含按一下hyper「前往完整清單」的選項，您將會被送到Salesforce中的新索引標籤，而MSI面板將會以全頁版面配置顯示
* 連絡人完整清單 — 不包含「前往完整清單」選項
* 連絡人行動裝置 — 顯示在Salesforce行動應用程式中
* 新增至Marketo Campaign ContactPage — 此面板中提供新增至Marketo Campaign功能

欄位：

* 上一個有趣的時刻
* 上一個有趣的時刻日期
* 上一個有趣時刻說明
* Source最後有趣的時刻
* 上一個有趣的時刻型別
* 最後一個Marketo活動（依銷售分列）
* 相對分數
* 相對分數值
* 急迫性
* 緊急值
* 在Marketo中檢視 — 按一下此欄位可開啟Marketo中潛在客戶的不可編輯檢視。 包括：銷售機會資訊、公司資訊、SFDC銷售機會資訊、SFDC自訂欄位、活動記錄
* Mkto銷售機會分數
* 銷售分析 — 開啟連絡人完整清單頁面

## 帳戶配置 {#account-layout}

Visualforce頁面：

* 帳戶 — 包含按一下「前往完整清單」的超選項，您將會被送到Salesforce中的新索引標籤，其中MSI面板將顯示在全頁版面配置中
* 帳戶完整清單 — 不包含「移至完整清單」選項
* 帳戶行動 — 顯示在Salesforce行動應用程式中

欄位：

* 銷售分析 — 開啟連絡人完整清單頁面

動作：

* 新增至Marketo Campaign
* 傳送Marketo電子郵件
* 新增/移除監看清單

下列功能在[帳戶配置]頁面中&#x200B;**無法使用**：

* 星星和火焰

## 機會配置 {#opportunity-layout}

Visualforce頁面：

* 商機 — 包含按一下hyper「前往完整清單」的選項，您將會被送到Salesforce中的新索引標籤，其中MSI面板將顯示在全頁版面配置中
* 機會完整清單 — 不包含「移至完整清單」選項
* Opportunity Mobile — 顯示在Salesforce行動應用程式中

欄位：

* 銷售分析 — 開啟連絡人完整清單頁面
* Marketo機會分析 — 在Marketo中開啟機會影響分析器

動作：

* 新增至Marketo Campaign
* 傳送Marketo電子郵件
* 新增/移除監看清單

下列功能在Opportunity Layout頁面中&#x200B;**無法使用**：

* 星星和火焰

## 潛在客戶與聯絡人清單檢視（大量動作） {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning：新增到觀察清單、新增到Marketo Campaign並在潛在客戶與聯絡人清單檢視中傳送Marketo電子郵件大量動作按鈕。

Salesforce Classic：新增到監看清單、新增到Marketo Campaign，以及在「銷售機會」和「連絡人清單」檢視中傳送Marketo電子郵件大量動作按鈕。

## Marketo索引標籤 {#marketo-tab}

* 首選

   * 包含建立和編輯檢視的功能。 可根據Marketo「設定」頁面中「預設隱藏」選項的設定，隱藏首選
   * 欄 — 名稱、帳戶、上一個有趣的時刻、狀態標題、參與（星星和火焰）、隱藏

* 我的觀察清單

   * 包含建立和編輯檢視的功能
   * 欄 — 名稱、帳戶、上一個有趣的時刻、狀態標題、參與（星星和火焰）、移除

* 網頁活動

   * 包括建立和編輯檢視的功能、時間範圍篩選功能
   * 欄 — 頁面檢視、名稱、帳戶、上次造訪

* 匿名網路活動

   * 包括建立和編輯檢視的功能、時間範圍篩選功能
   * 欄 — 頁面檢視、公司、上次造訪、研究(開啟公司的LinkedIn頁面)

* 我的電子郵件

   * 包含建立和編輯檢視的功能
   * 欄 — 名稱、帳戶、主旨、日期、開啟、按一下

* 潛在客戶摘要 — 包含訂閱有趣時刻的功能，設定頁面上的RSS摘要必須啟用才能使用此功能

   * 有這個有趣時刻的主管/聯絡人
   * 有趣的時刻型別（網頁、電子郵件或里程碑）和說明
   * 帳戶名稱
   * 這個有趣時刻發生的時間
   * 訂閱選項以接收此類事件的電子郵件通知
   * 高優先順序圖示可顯示此人員為最佳匹配

## Marketo Sales Insight設定索引標籤 {#marketo-sales-insight-configuration-tab}

* 操作設定：包含在SFDC中設定MSI所需的Soap與Rest API認證
* MSI設定：包含Marketo索引標籤和MSI Visualforce面板的設定
* 重設Marketo Sales Insight：包含清除所有設定的功能

>[!MORELIKETHIS]
>
>[Salesforce中的Marketo Sales Insight設定索引標籤](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## 銷售分析績效報表 {#sales-insight-performance-reports}

檢視透過Salesforce、Microsoft Dynamics或Gmail或Outlook外掛程式傳送的電子郵件效能

## 適用於行動裝置的MSI {#msi-for-mobile}

Salesforce行動應用程式支援MSI功能

## 語言支援 {#language-support}

Marketo Sales Insight是依語言儲存。 因此，如果您希望它適用於多種語言，則必須分別輸入每種語言的認證。

>[!NOTE]
>
>* 連絡人/潛在客戶必須位於「預設」分割中，才能新增至「監看清單」。
>
>* MSI Salesforce套件不支援具有相依欄位的自訂檢視。
