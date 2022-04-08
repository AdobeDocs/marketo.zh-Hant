---
unique-page-id: 42762322
description: MarketoSales Force中的Sales Insight配置頁籤 — Marketo文檔 — 產品文檔
title: MarketoSales Insight配置頁籤（在Salesforce中）
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# MarketoSales Insight配置頁籤（在Salesforce中） {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作設定 {#operational-settings}

您需要設定此設定，以便開始在SFDC中使用Sales Insight。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI同時使用Soap和Rest API
* 您的Marketo帳戶中的Sales Insight頁面將有兩個相應的面板，其中包含您可以在此處複製和貼上的Soap和Rest API憑據
* Soap和Rest API有單獨的超時時間，您可以根據組織的需要設定這些超時時間。 允許的最長時間為120秒
* 禁用Insights儀表板：您可以刪除Rest API憑據，並且只能使用Soap API。 這樣做將禁用所有MSI視力面板中的Insights Dashboard頁籤

## MSI配置 {#msi-configuration}

配置適用於所有MSI用戶，並且不特定於配置檔案。

**VisualForce頁面設定**

* 啟用操作下拉清單：
   * 能夠隱藏在潛在客戶和聯繫MSI佈局中的下拉清單中發送Marketo電子郵件
   * 能夠隱藏「添加到Marketo市場活動」選項，使其不在銷售線索和聯繫MSI佈局中下拉
* 即將發生的事件：能夠向用戶顯示邀請的事件、所有事件或完全隱藏此頁籤
* 即將推出的活動：能夠顯示所有電子郵件活動或完全隱藏此頁籤
* 載入即將進行的市場活動和事件：通過將事件和市場活動標籤置於按需「載入即將到來的項目」按鈕後，減少用戶調用的剩餘API數
* 頁籤設定：預設情況下，所有五個頁籤都可用。 您可以在「銷售透視」面板中選擇標籤的順序。 同一訂單將適用於所有佈局（銷售線索、聯繫人、客戶、業務機會）

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Marketo全局頁籤**

* 已啟用RSS源：啟用後，MSI用戶可以在RSS源中查看其Lead Feed（除Salesforce中的Lead Feed外）。 RSS源只有在禁用「令牌過期」功能時才能運行。 此設定在您的MarketoSales Insight Admin頁中控制。
* 最佳調試模式
* 預設隱藏：您在此處選擇的選項是當您按一下「隱藏」表徵圖時，在Marketo的「最佳匹配」頁籤中隱藏最佳匹配的天數
* 聯繫人狀態欄位：您在此處選擇的選項是在Marketo「最佳匹配」頁籤的「狀態標題」列中填充的值
* 即時源設定：選擇只顯示Live Feed(在Lead、Contact、Account和Opportunity面板以及全球Marketo頁中)、Lead Feed(在Marketo全球頁中)或Live和Lead Feed
* 頁籤設定：預設情況下，所有五個頁籤都可用。 可以選擇Marketo全局頁中的頁籤順序

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**限制**

* 預設情況下，「活動」(Interest Moment, Web Activity, E-mail)設定為1000。 預設情況下，電子郵件市場活動和事件設定為200
* 如果您注意到組織上存在超時問題，您可以降低限制

**操作設定**

* 發送Marketo電子郵件：啟用此功能將使所有Sales Insight用戶都能夠訪問Lead 、 Contact 、 Account 、 Opportunity面板和Best Bets頁籤（批量操作和內聯接洽）中發送電子郵件
* 添加到Marketo市場活動：啟用此功能將使所有Sales Insight用戶都可以訪問Lead 、 Contact 、 Account 、 Opportunity面板和Best Bets頁籤（批量操作和內聯參與）中的市場活動

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## 重置Marketo銷售洞察 {#reset-marketo-sales-insight}

選擇這樣做將擦除SFDC中的所有配置，並且無法恢復這些配置。 您必須重新配置所有內容。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!IMPORTANT]
>
>除非您使用Sales Insights Actions功能，否則不要選中「啟用MSI操作」複選框。

>[!MORELIKETHIS]
>
>[將Sales Insight訪問權添加到配置檔案](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;
