---
description: 當前發行說明 — Marketo文檔 — 產品文檔
title: 當前發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 87410bcdc5f9ebb3b85765efe9fd852df4611ce6
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# 發行說明：2022年1月 {#release-notes-jan-22}

2022年1月的發行版包含以下功能。 檢查您的AdobeMarketo Engage版以瞭解功能可用性。

>[!AVAILABILITY]
>
>用星表示的特徵(![星](assets/yellow-star.png))是付費附加項。 請聯繫您的Marketo Engage代表以瞭解詳細資訊。

**_季度發佈_**

以下功能將開始在 **2022年1月21日**，在接下來的幾週內（除非另有指定）分階段部署每項功能。

## 新一代體驗 {#next-generation-experience}

* **新一代體驗中的更新螢幕**:我們將提供新一代體驗中的更多刷新螢幕，提供可通過切換開關進行的更新設計和可用性增強：

   * Design Studio中的登錄頁資產詳細資訊
   * 市場營銷活動中的登錄頁資產詳細資訊

## Microsoft動力學整合 {#microsoft-dynamics-integration}

* **多選選項集欄位類型的同步通常可用**:從MicrosoftDynamics同步多選選項集欄位類型，以便在智慧清單和智慧市場活動中利用，以針對更細粒度的受眾。 示例包括：主題/產品、首選的通信模式等。 此新同步適用於MicrosoftDynamics 9.X版（包括Dynamics 365線上版）。

* **用於MicrosoftDynamics 365線上的伺服器到伺服器身份驗證**:為了提高安全性，我們現在將支援伺服器到伺服器(S2S)，作為Azure Active Directory上Marketo Engage同步用戶的附加身份驗證模式，以便對MicrosoftDynamics 365 Online進行非互動式訪問。 這允許您使用多重身份驗證，因為所有身份驗證和登錄都將基於OAuth（僅客戶端ID和客戶端機密）。

>[!NOTE]
>
>S2S模式基於應用程式用戶而不是授權用戶，這樣可節省額外許可證的使用。

## 管理 {#administration}

* **[表單驗證規則](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**:通過阻止有問題或不希望的電子郵件域提交Marketo Engage表，維護資料庫的運行狀況。 「全局表單驗證規則」面板允許管理員定義阻止清單或啟用預定義的自由使用者域清單以阻止表單。

* **[登錄頁標題安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**:管理員可以在其登錄頁域上管理嚴格傳輸安全性和X-Frame選項標題，以強制執行強大的安全要求。

**_在整個季度發佈_**

以下功能處於非季度週期，將在未來幾個月中發佈。

## AEPMarketo Engage目標連接器 — 建立新銷售線索 {#aep-marketo-engage-destination-connector}

Marketo Engage也使用Adobe Experience Platform(AEP)的客戶可以通過AEP目標連接器將新人記錄從AEP推送到Marketo Engage中，從而最大限度地提高其資料庫的利用率。 在將受眾段從AEP發送到Marketo Engage時，該段內尚不存在於您的Marketo Engage資料庫中的人員 [可以自動添加到](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## 銷售洞察 {#sales-insight}

![（星號）](assets/yellow-star.png)

**Sales Insight for Salesforce CRM**

* **用於最佳匹配的新類型列**:賣家將通過標有「類型」的新專欄獲得更快的洞察力，以在「最佳賭注」頁面上區分銷售線索和聯繫人。

* **Salesforce平台API更新**:為響應Salesforce退出Salesforce平台API版本21.0到30.0,Sales Insight包已使用最新API進行更新。

* **更新的品牌**:正在更新所有Sales Insight頁面，以與Adobe品牌相協調。

**Microsoft動力的銷售洞察**

* **已更新的帳戶佈局**:賣家可以集體瞭解頂級活動，例如：電子郵件活動、Web活動、有趣時刻以及帳戶內所有聯繫人的評分更改。

## 銷售連接 {#sales-connect}

![（星號）](assets/yellow-star.png)

* **呼叫結果和原因**:通過全新、完全可定製的呼叫結果和呼叫原因選項，更詳細地瞭解和跟蹤銷售團隊的出站工作。 除了這些新欄位外，我們還引入新的管理機制，在銷售商進行呼叫時強制執行呼叫原因和結果選擇，啟用或禁用呼叫原因和結果的新治理機制，以及新的呼叫原因和呼叫結果Salesforce活動自定義欄位，用於將資料記錄到Salesforce。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) 來瞭解更多資訊。

* **Salesforce活動詳細資訊自定義**:通過自定義當銷售活動從Sales Connect記錄到Salesforce時將哪些資訊添加到Salesforce任務主題欄位，在Salesforce中捕獲更多銷售活動和任務資料。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) 來瞭解更多資訊。

## 公告 {#announcements}

* **Marketo Sky棄用**:3月11日，Marketo Sky將不再可用，因為我們將資源集中在提供下一代用戶體驗上。 為了保持對目前Marketo Sky獨有功能的訪問，我們將在3月份將資產到期和智慧市場活動優先順序改寫納入主流體驗。 [按一下這裡](https://nation.marketo.com/t5/the-next-generation-experience/marketo-sky-deprecation-notice/ba-p/320115#M33) 來瞭解更多資訊。

* **表單終結點棄用**:不支援的寫程式表單POST到leadCapture/save2終結點，將被Marketo Engage表單拒絕。 [按一下這裡](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) 來瞭解更多資訊。

* **電子郵件驗證**:從此版本後開始，Marketo Engage訂閱將開始讓「非API」用戶驗證電子郵件地址。 當使用「電子郵件驗證」啟用訂閱時，經目錄服務驗證的用戶將自動驗證其電子郵件。 使用「登錄邀請用戶對話框」功能的用戶或訂閱中具有與訂閱內的多個用戶關聯的單個電子郵件的用戶的電子郵件驗證將延遲，並與該功能在3月棄用的時間一致。

* **在「邀請用戶」對話框中登錄**:3月，現有的可選功能「登錄邀請用戶對話框」將被棄用。 「登錄邀請用戶對話」功能被通用ID功能覆蓋，該功能是即將Adobe的Identity Management系統整合所必需的，於2021年8月在所有訂閱上啟用。 由於出現棄用，Marketo Engage將只強制一個用戶在訂閱內按電子郵件地址關聯。

**Marketo Engage域 — Sales Insight配置**:對於未設定SSL證書的Marketo Engage域和https://，調用將失敗，並出現SSL握手錯誤。 因此，這些域將會落日。 因此，指向這些域中任何一個的較舊配置的Sales Insight用戶在其Lead 、 Contact 、 Account 、 Opportunity Panels或MarketoGlobal頁面上可能會遇到系統標注錯誤。 我們建議您更新 [Marketo Engage配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 在Salesforce中。 您只需更新文檔「Marketo銷售洞察力配置」部分中突出顯示的Marketo Engage憑據。

**_產品發佈網路研討會_**

2022年1月27日，美國東部時間上午9:00/下午12:00 [即時網路研討會](https://engage.marketo.com/2022_January_Release_Webinar_RegistrationPage.html) 由我們的產品團隊主持，您可以在此學習如何使用所有最新的產品創新。
