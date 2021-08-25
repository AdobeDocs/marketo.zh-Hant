---
description: 最新發行說明 — Marketo檔案 — 產品檔案
title: 最新發行說明
source-git-commit: 6f9b5a591a315fd6ff036cd5d51dbb432bd31733
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 0%

---

# 發行說明：2021年8月 {#release-notes-aug-21}

』21年8月發行包含下列功能。 查看您的Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))表示的功能為付費附加元件。 請連絡您的AdobeMarketo Engage代表以了解更多資訊。

**_每季發行_**

下列功能將於2021年8月20日發行&#x200B;****。

## 體驗自動化 {#experience-automation}

* **Marketo Engage使用者透過Adobe身分驗證**:自2021年9月起，將使用Adobe ID使用者認證，上線具有企業套件的新Marketo Engage使用者。到2022年年中，目前的使用者才會移轉至整合身分系統，在進一步通知前，不需要採取任何動作。 Adobe身分使用者驗證可讓IT/安全管理員管理多個Marketo Engage產品例項以及其他Experience Cloud解決方案，以及透過通用主控台設定SSO。 管理員可以方便地在一個位置管理使用者群組和使用者權益。

* **可執行的促銷活動巢狀**:可執行的促銷活動現在也可以呼叫其他可執行的促銷活動，讓您最多巢狀內嵌至三個層級。這可以進一步整合常見的操作流程，並改進Smart Campaign管理。

* **「人員詳細資料」頁面中的「單一流量動作** 」（9月9日前推出）:使用「流程操作」菜單，從人員詳細資訊頁對個人執行流操作，如發送電子郵件、更改人員所有者或任何其他智慧促銷活動操作，而不切換到資料庫網格視圖。

* **[自訂活動匯出](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**:中繼資料匯出現在支援所有物件和個別中繼資料，可用來共用、分析和設計您的訂閱資料模型。

## API增強功能 {#api-enhancements}

* **提交表單API**:當一個電子郵件地址在兩個或多個Lead記錄中重複時，我們會更新「上次更新」記錄，而非完全略過。提供與Forms 2.0 API同等的支援。

* **電子郵件API**:擷取冠軍或挑戰者電子郵件資產。使用日期範圍篩選器擷取電子郵件資產。

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

* **增強Salesforce CRM使用者對銷售機會、連絡人、帳戶和商機活動的可見度**:在較長的銷售週期中與潛在客戶的接洽會更加了解，因為Sales Insight中的參與記錄數量增加。有趣的時刻、Web活動、電子郵件和分數頁簽在Lead、Contact、Account和Opportunity對象中顯示多達400個活動。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **電子郵件連線限制（測試版）**:利用Sales Connect的電子郵件連線限制，改善電子郵件傳遞能力並擴展個人化銷售通訊。這項新技術可自動管理電子郵件傳送時間，為Exchange和Gmail使用者建立順暢的體驗。 減少或消除第三方批量電子郵件發送應用程式的使用，並信心十足地從Sales Connect發送您的所有電子郵件。

>[!NOTE]
>
>現在，測試版已提供電子郵件限制功能。 [更多詳情](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

* **增強銷售活動分析**:根據您銷售團隊的先前活動，擷取並啟用個人化參與。新屬性（如「銷售呼叫記錄連結」、「銷售促銷活動名稱」和「銷售電子郵件主體」）可用於Marketo Engage智慧清單。  這些活動可透過「Marketo EngageREST API」或「大量匯出」來匯出和報告，並可在篩選器和觸發器上使用，作為智慧清單的其他限制。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms整合**:行銷人員現在可以針對LinkedIn透過其Lead Gen Forms廣告單位擷取表單填入時發生的轉換，執行收入歸因。然後，這些見解便可用來最佳化表單效能和付費媒體投資。 linkedIn Lead Gen Forms是LinkedIn增長最快的付費媒體產品之一，此新功能包含在我們與Bizible的現有LinkedIn Ads整合中。 
 
* **改良的Velocity控制面板**:我們新增了新的速度量度和控制面板篩選器，以提供更深入的分析。此控制面板供行銷人員用來了解各階段的銷售機會和商機速度，以及不同行銷和銷售互動形式的效率。

* **新的同類群組瀑布歷程控制面板**:這可讓行銷人員透過經典的「需求瀑布圖」階段集來檢視所選同類群組的進展，進而快速了解轉換率，並逐階段隱含階段轉換因果關係。

## Bizible與Adobe Experience Cloud整合 {#bizible-integration-with-adobe-experience-cloud}

本節包含已完成AdobeIdentity Management系統(IMS)移轉的Bizible使用者的新功能。 如果您已移轉，您會在「Adobe ID」標籤下的「Bizible Settings」中看到新的Adobe ID。 所有帳戶應在2021年底前移轉。

* **Bizible與AdobePrivacy Service整合** （2021年9月推出）:Bizible與AdobePrivacy Service的整合可集中Adobe Experience Cloud應用程式對重要資料隱私權法規（例如GDPR）的遵循。您現在可以善用此服務並集中管理所有隱私權要求，以便在應用程式間反映傳入Bizible和其他Adobe產品的變更要求。

* **Adobe統一殼層上的Bizible**:Bizible採用AdobeUnified Shell為用戶提供了新功能，這些功能將出現在Bizible應用程式標頭欄中，並包括更好地訪問支援資源和應用程式切換。AdobeUnified Shell可協助在Bizible與其他Adobe Experience Cloud應用程式之間建立一致的體驗。

* **Bizible網域所有權與自我管理**:Bizible使用者可運用Adobe Admin Console來管理他們希望Bizible追蹤的網域。這為先前的手動程式提供自助服務，並提供如何跨Adobe Experience Cloud應用程式管理網域擁有權和追蹤的一致體驗。

## 公告 {#announcements}

* **訂閱通用ID設定的更新**:為支援現有使用者即將推出的Marketo Engage與Adobe身分整合，所有Marketo Engage訂閱將透過啟用通用ID支援統一。
