---
unique-page-id: 42762322
description: Salesforce中的Marketo Sales Insight設定索引標籤 — Marketo檔案 — 產品檔案
title: Salesforce中的Marketo Sales Insight設定索引標籤
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 4848676d423ff96c2e880819bc760b2f8dbbd094
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Salesforce中的Marketo Sales Insight設定索引標籤 {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作設定 {#operational-settings}

您必須設定此專案，才能開始在SFDC中使用Sales Insight。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI同時使用Soap和Rest API
* 您的Marketo帳戶中的「銷售分析」頁面會有兩個相對的面板，各具有Soap和Rest API認證，您可以在此處複製和貼上
* Soap和Rest API有不同的逾時，您可以根據組織的需求加以設定。 允許的時間上限為120秒
* 停用前瞻分析控制面板：您可以移除Rest API認證，而只使用Soap API。 這麼做會停用所有MSI Visualforce面板中的「前瞻分析儀表板」索引標籤

## MSI設定 {#msi-configuration}

設定適用於所有MSI使用者，而非設定檔專用。

**Visualforce頁面設定**

* 啟用動作下拉式清單：
   * 能夠隱藏潛在客戶與聯絡MSI配置中的下拉式清單中的「傳送Marketo電子郵件」
   * 能夠隱藏潛在客戶與聯絡MSI配置中下拉式清單的「新增至Marketo促銷活動」選項
* 即將到來的活動：向使用者顯示已邀請的活動、所有活動或完全隱藏此索引標籤的功能
* 即將推出的行銷活動：顯示所有電子郵件行銷活動或完全隱藏此索引標籤的功能
* 載入即將到來的行銷活動和事件：將事件和行銷活動索引標籤放置在隨選「載入即將到來的專案」按鈕後面，能夠減少使用者發出的Rest API呼叫數量
* 索引標籤設定：預設狀態下將可使用全部五個索引標籤。 您可以在「銷售分析」面板中選擇索引標籤的順序。 相同的順序將適用於所有配置（銷售機會、連絡人、客戶、商機）

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Marketo全域標籤**

* 啟用RSS摘要：啟用時，MSI使用者可以在RSS摘要中檢視其銷售機會摘要（除了Salesforce中的銷售機會摘要之外）。 RSS摘要只有在「權杖有效期」功能停用時才有作用。 此設定是在您的Marketo Sales Insight 「管理員」頁面中控制。
* Best Bets偵錯模式
* 預設隱藏：您在此處選擇的選項為按一下「隱藏」圖示時，Marketo中「首選」索引標籤中隱藏的天數
* 連絡人狀態列位：您在此處選擇的選項將會是在Marketo中「首選」索引標籤的「狀態標題」欄中填入的值
* 即時摘要設定：選擇只顯示即時摘要(在「銷售機會」、「聯絡人」、「帳戶」和「機會」面板，以及「全域Marketo」頁面中)、只顯示銷售機會摘要(在「Marketo全域」頁面中)或同時顯示即時和銷售機會摘要的選項
* 索引標籤設定：預設狀態下將可使用全部五個索引標籤。 您可以在Marketo全域頁面中選擇索引標籤順序

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**限制**

* 活動（有趣的時刻、網頁活動、電子郵件）預設為1000。 電子郵件行銷活動和事件預設為200
* 如果您發現組織發生逾時問題，您可以降低限制

**動作設定**

* 傳送Marketo電子郵件：啟用此項可讓所有Sales Insight使用者從Lead、Contact、Account、Opportunity面板和Best Bets索引標籤（大量動作和內嵌參與）傳送電子郵件
* 新增至Marketo Campaign：啟用此項可讓所有Sales Insight使用者從Lead、Contact、Account、Opportunity面板和Best Bets索引標籤（大量動作和內嵌參與）新增至行銷活動

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## 支援設定 {#support-settings}

選取此核取方塊將會在您的Salesforce執行個體中啟用偵錯記錄。 它有助於您疑難排解問題。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## 重設Marketo Sales Insight {#reset-marketo-sales-insight}

若選擇這麼做，將會清除SFDC中的所有設定，且無法還原。 您必須重新設定所有專案。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>除非您使用銷售分析動作功能，否則請勿選取「啟用MSI動作」核取方塊。

>[!MORELIKETHIS]
>
>[將銷售分析存取權新增至設定檔](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
