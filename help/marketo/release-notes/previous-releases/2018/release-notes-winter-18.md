---
unique-page-id: 13795395
description: 發行說明 — 冬季』18年 — Marketo檔案 — 產品檔案
title: 發行說明 — 2018年冬季
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# 發行說明：2018 年冬季 {#release-notes-winter}

以下功能包含在2018年冬季發行版本中。 檢查您的Marketo版本是否有功能可用。

請按一下標題連結以檢視每個功能的詳細文章。 **注意**：此版本中包含的部分功能沒有相關文章。 如果主題有多個副標題，連結就會放在那裡。

## 行銷活動效能和輸送量增強功能 {#campaign-performance-and-throughput-enhancements}

Marketo運用我們的大型資料架構，提高觸發行銷活動的輸送量，並改善網路活動處理，讓您更迅速地回應對象的動作。

## Marketo [!DNL Salesforce] CRM整合的增強功能 {#enhancements-to-marketo-s-salesforce-crm-integration}

我們的[!DNL Salesforce] CRM整合有兩項增強功能：

* 針對某些CRM同步處理失敗（憑證過期、達到API限制等），[Marketo管理員通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)

* [可在潛在客戶指派時關閉潛在客戶擁有者的電子郵件通知](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md)

這些改善將於2018年推出。

## [Marketo效能深入分析](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>[!UICONTROL Performance Insights]是附加產品。 如需報價，請聯絡您的Marketo客戶成功經理或客戶主管。

透過Attribution Analytics、互動式視覺效果和詳細的資料表格，探索行銷活動和管道如何影響業務結果。

![](assets/image2018-2-5-7-3a55-3a46.png)

## 帳戶型行銷增強功能 {#account-based-marketing-enhancements}

**[ABM階層](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

對於具有[!DNL Salesforce]或[!DNL Microsoft Dynamics]的ABM客戶，ABM現在將自動繼承（及顯示）在CRM中建立的父子關係。 您就可以在統計報表和行銷活動執行中使用這些關係。

## 電子郵件行銷 {#email-marketing}

**[動態電子郵件指令碼](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

使用動態內容的電子郵件現在支援Velocity指令碼。 結合速度和分段型動態內容，建立高度個人化的電子郵件。

**收件者時區**

* **[每月的Nurture Cadence](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**：我們已新增每月排程Nurture計畫的功能。

* **[停止傳遞](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**：您現在可以停止任何剩餘的傳送中繼。

## 廣告網路整合 {#ad-network-integrations}

**[Google Customer Match整合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

透過這項整合，您可以傳送Marketo對象至Google以使用[!DNL Google AdWords]定位，以及跨[!DNL YouTube]、搜尋和[!DNL Gmail]重新定位對象。

**[[!DNL LinkedIn] 相符的Audiences API增強功能](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

我們的新[!DNL LinkedIn] API現在可讓您跨多個[!DNL LinkedIn]行銷活動經理帳戶，重新鎖定Marketo資料庫中的人員。

## 網頁個人化 {#web-personalization}

適用於Web Personalization的&#x200B;**Japanese Data Source**

Marketo正在新增另一個日本資料來源用於Web Personalization，以改進來自日本的訪客的網站訪客識別（反向IP查詢）和個人化。 組織名稱會顯示為日文。

**[使用靜態清單建立網頁區段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization現在可以將內容個人化給屬於行銷活動(MLM)中定義的靜態清單一部分的已知網頁訪客。 透過此增強功能，您現在可以跨管道行銷靜態清單，並以您網站上的個人化內容來鎖定這些清單上的人員。

## ContentAI {#contentai}

**預測演演算法改進**

透過Marketo最佳化ContentAI演演算法的建議內容所產生的點按次數，是隨機內容的兩倍。

## 整合 {#integration}

**[啟用/停用行銷活動API](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

此新API可讓您從遠端啟用和停用觸發程式行銷活動，因此您現在可以建立完全自動化的方案範本。 一次建立方案範本，然後自動複製、行銷宣傳品更新，現在則啟動/排程智慧型行銷活動。

## [!DNL ToutApp] {#toutapp}

**取消訂閱更新**

自2018年3月1日起，從[ToutApp.com](https://ToutApp.com)傳送的所有電子郵件（以及使用[!DNL Tout]中的[包含[!DNL Salesforce]的電子郵件]按鈕）底部都會附加一個取消訂閱連結。

**即時摘要更新**

我們已更新「參與」和「任務」標籤的外觀和風格，讓銷售成員可以更快、更輕鬆的方式直接從即時摘要回應客戶活動。

**人員詳細資料檢視更新**

改善的人員詳細資料檢視(PDV)將您的[!DNL Tout]和[!DNL Salesforce] CRM連絡人詳細資料彙集在一起，提供您連絡人的完整檢視。
