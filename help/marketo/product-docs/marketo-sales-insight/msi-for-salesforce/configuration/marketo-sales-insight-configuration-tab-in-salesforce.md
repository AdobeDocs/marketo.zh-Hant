---
unique-page-id: 42762322
description: Salesforce中的Marketo Sales Insight設定標籤- Marketo Docs —— 產品檔案
title: Salesforce中的Marketo Sales Insight「設定」標籤
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}中的Marketo Sales Insight設定標籤

## 操作設定{#operational-settings}

您需要進行此設定，才能開始使用SFDC中的Sales Insight。

![](assets/one.png)

* MSI同時使用Soap和Rest API
* 您Marketo帳戶中的「銷售分析」頁面將有兩個對應的面板，其中包含Soap和Rest API憑證，您可在此處複製和貼上
* Soap和Rest API有個別的逾時，您可以根據組織的需求加以設定。 允許的最大時間為120秒
* 停用前瞻分析控制面板：您可以移除Rest API認證，而且只能使用Soap API。 這麼做會停用所有MSI視覺強制面板中的「前瞻分析控制面板」標籤

## MSI配置{#msi-configuration}

配置適用於所有MSI用戶，並且不特定於配置檔案。

**行銷人員標籤設定**

* 最佳除錯模式
* 預設隱藏——您在此處選擇的選項是當您按一下「隱藏」圖示時，最佳賭注將隱藏在Marketo的「最佳押注」索引標籤中的天數
* 連絡人狀態欄位——您在此處選擇的選項是填入Marketo中「最佳押注」標籤之「狀態標題」欄中的值
* 標籤設定——預設會提供所有5個標籤。 您可以在Marketo全域頁面中選擇標籤順序

**Visualforce頁面設定**

* 啟用動作下拉式清單：

   * 能夠隱藏銷售機會與連絡人MSI配置中的「傳送行銷人員電子郵件」下拉式清單
   * 能夠隱藏「新增至行銷人員促銷活動」選項，避免「銷售機會與連絡人MSI配置」下拉式清單中的問題

* 近期活動：能夠向使用者顯示邀請的事件、所有事件或完全隱藏此標籤
* 近期促銷活動：可顯示所有電子郵件促銷活動或完全隱藏此標籤
* 載入即將推出的促銷活動和事件：透過將事件和促銷活動標籤置於隨選「載入即將進行的項目」按鈕後，可減少使用者進行的Rest API呼叫次數
* 標籤設定——預設會提供所有5個標籤。 依預設，所有5個標籤皆可使用。 您可以在Sales Insight面板中選擇標籤順序。 相同的訂單將適用於所有版面（銷售機會、聯絡人、帳戶、業務機會）

![](assets/two.png)

**限制**

* 活動（「有趣的時刻」、「網頁活動」、「電子郵件」）預設為1000。 電子郵件促銷活動和事件預設為200
* 如果您發現組織上的逾時問題，可以降低

## 重設Marketon Sales Insight {#reset-marketo-sales-insight}

選擇這樣做將擦除SFDC中的所有配置，並且無法恢復這些配置。 您必須重新設定所有項目。

![](assets/three.png)

>[!MORELIKETHIS]
>
>[為您的團隊設定銷售分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
