---
description: 發行說明 — 2021年8月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2021年8月
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 發行說明： 2021年8月 {#release-notes-aug-21}

2021年8月發行版本包含下列功能。 檢查您的Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))為付費附加元件。 請聯絡您的Adobe Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將會發行日期 **2021年8月20日**.

## 體驗自動化 {#experience-automation}

* **透過Adobe身分進行Marketo Engage使用者驗證**：不久，將使用Adobe ID使用者認證來上線具有企業套件的新Marketo Engage使用者。 2022年中之前不會將目前的使用者移轉至整合式身分系統，在進一步通知之前不需要採取任何動作。 Adobe身分使用者驗證可讓IT/安全管理員管理多個Marketo Engage產品執行個體及其他Experience Cloud解決方案，並透過通用主控台設定SSO。 管理員可以在一個地方方便地管理使用者群組和使用者權益。

* **可執行檔行銷活動巢狀**：可執行行銷活動現在也可以呼叫其他可執行行銷活動，讓您最多可在三個層級深度巢狀內嵌這些行銷活動。 如此可進一步整合常見作業流程，並改善Smart Campaign管理。

* **個人詳細資料頁面中的單一流程作業** （9月9日前提供）：在不切換至資料庫網格檢視的情況下，使用流程動作選單從人員詳細資料頁面執行流程動作，例如傳送電子郵件、變更人員擁有者或針對個別人員執行任何其他智慧行銷活動動作。

* **[自訂活動匯出](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**：中繼資料匯出現在支援所有物件和個別中繼資料，可用於共用、分析和設計您的訂閱資料模型。

## API增強功能 {#api-enhancements}

* **提交表單API**：當電子郵件地址在兩個或多個Lead記錄中重複時，我們會更新「上次更新」記錄而不是完全跳過。 提供與Forms 2.0 API的同等功能。

* **電子郵件API**：擷取冠軍或挑戰者電子郵件資產。 使用日期範圍篩選器擷取電子郵件資產。

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## 銷售分析 {#sales-insight}

![（星號）](assets/yellow-star.png)

* **增強Salesforce CRM使用者的Lead、Contact、Account和Opportunity活動的可見度**：由於Sales Insight中的參與記錄數量增加，在漫長的銷售週期中與潛在客戶互動時可獲得更多資訊。 有趣的時刻、網頁活動、電子郵件和分數標籤會顯示Lead、Contact、Account和Opportunity物件中最多400個活動。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **電子郵件連線節流（測試版）**：使用Sales Connect的電子郵件連線節流功能，改善電子郵件傳遞能力並擴展個人化銷售通訊。 這項新技術會自動管理電子郵件傳送時間，為Exchange和Gmail使用者創造順暢的體驗。 減少或避免使用協力廠商大量電子郵件傳送應用程式，並放心地從Sales Connect傳送所有電子郵件。

>[!NOTE]
>
>電子郵件節流功能現在可在Beta版中使用。 [深入了解](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **增強的銷售活動深入分析**：根據您的銷售團隊先前的活動，擷取並啟用個人化參與。 新的屬性（例如「銷售電話錄音」連結、銷售行銷活動名稱和銷售電子郵件主旨）可用於Marketo Engage智慧清單。  這些活動可透過Marketo EngageREST API或大量匯出來匯出和報告，並可在篩選器和觸發器上作為智慧清單的額外限制使用。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms整合**：行銷人員現在可以對LinkedIn透過其Lead Gen Forms廣告單位擷取表單填入時發生的轉換執行收入歸因。 這些見解可用於最佳化表單效能和付費媒體投資。 linkedIn Lead Gen Forms是LinkedIn增長最快的付費媒體產品之一，這項新功能包含在我們與Bizible的現有LinkedIn Ads整合中。

* **改善的Velocity儀表板**：我們已新增速度量度和控制面板篩選器，能提供更深入的見解。 此儀表板可供行銷人員用來瞭解逐階段銷售線索和機會速度，以及不同形式行銷和銷售參與的效率。

* **新同類群組Waterfall歷程儀表板**：這可讓行銷人員檢視選定同類群組在傳統「需求瀑布」階段集中的進度，進而提供對轉換率和隱含階段轉換因果關係的逐階段快速瞭解。

## Bizible與Adobe Experience Cloud整合 {#bizible-integration-with-adobe-experience-cloud}

本節包括已完成其AdobeIdentity Management System (IMS)移轉的Bizible使用者適用的新功能。 如果您已移轉，您會在Adobe ID標籤下方的Bizible設定中看到新的Adobe ID。 所有帳戶應於2021年底移轉。

* **Bizible與AdobePrivacy Service整合** （2021年9月推出）： Bizible與AdobePrivacy Service的整合可跨Adobe Experience Cloud應用程式集中遵循關鍵資料隱私權法規（例如GDPR）。 您現在可以善用此服務，集中管理所有隱私權請求，好讓所有應用程式都能反映傳入Bizible和其他Adobe產品的變更請求。

* **Adobe Experience Cloud介面上的Bizible**： Bizible採用Adobe Experience Cloud介面，讓使用者擁有新功能，這些功能會顯示在Bizible應用程式標題列中，且包含支援資源和應用程式切換的更佳存取權。 Experience Cloud介面有助於在Bizible和其他Adobe Experience Cloud應用程式之間建立一致的體驗。

* **Bizible網域擁有權和自我管理**： Bizible使用者可運用Adobe Admin Console管理他們希望Bizible追蹤的網域。 這可為先前手動的流程帶來自助服務，並提供如何跨Adobe Experience Cloud應用程式管理網域擁有權和追蹤的一致體驗。

## 公告 {#announcements}

* **更新訂閱通用ID設定**：為了支援現有使用者即將推出的Marketo Engage和Adobe身分整合，所有Marketo Engage訂閱都將在啟用通用ID支援時統一。 更多資訊 [可在此處找到](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_產品發行網路研討會_**

[2021年8月Marketo Engage發行網路研討會](https://engage.marketo.com/August21_Release_Webinar.html)
