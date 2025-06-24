---
description: 發行說明 — 2021年8月 — Marketo檔案 — 產品檔案
title: 版本注意事項 - 2021 年 8 月
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# 發行說明： 2021年8月 {#release-notes-aug-21}

2021年8月發行版本包含下列功能。 檢查您的Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))表示的功能是付費附加元件。 請聯絡您的Adobe Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將於&#x200B;**2021年8月20日**&#x200B;發行。

## 體驗自動化 {#experience-automation}

* **透過Marketo Engage Identity進行Adobe使用者驗證**：不久將使用Adobe ID使用者認證來上線具有Enterprise套件的新Marketo Engage使用者。 目前的使用者要到2022年年中才會移轉至整合式身分系統，而且除非另行通知，否則不需要採取任何動作。 Adobe身分使用者驗證可讓IT/安全管理員管理多個Marketo Engage產品執行個體及其他Experience Cloud解決方案，並透過通用主控台設定SSO。 管理員可以在一個位置方便地管理使用者群組和使用者權益。

* **可執行促銷活動巢狀內嵌**：可執行促銷活動現在也可以呼叫其他可執行促銷活動，讓您最多可將其巢狀內嵌至三層深。 這可進一步整合常見作業流程，並改善Smart Campaign管理。

* **個人詳細資料頁面中的單一流量動作** （9月9日前提供）：在不切換至資料庫網格檢視的情況下，使用流量動作選單在個人詳細資料頁面中針對個別人員執行流量動作，例如傳送電子郵件、變更個人擁有者或任何其他智慧促銷活動動作。

* **[自訂活動匯出](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**：中繼資料匯出現在支援所有物件和個別中繼資料，這些物件和中繼資料可用來共用、分析和設計您的訂閱資料模型。

## API增強功能 {#api-enhancements}

* **提交表單API**：當電子郵件地址在兩個或更多潛在客戶記錄中重複時，我們會更新「上次更新」記錄而不是完全跳過。 提供與Forms 2.0 API的同等功能。

* **電子郵件API**：擷取冠軍或挑戰者電子郵件資產。 使用日期範圍篩選器擷取電子郵件資產。

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* **Salesforce CRM使用者的Lead、Contact、Account及Opportunity活動可見度提升**：由於[!DNL Sales Insight]中的參與記錄數量增加，在長銷售週期期間與潛在客戶互動會更明智。 有趣的時刻、網頁活動、電子郵件和分數索引標籤會顯示Lead、Contact、Account和Opportunity物件中最多400個活動。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **電子郵件連線節流(Beta)**：使用Sales Connect的電子郵件連線節流，改善電子郵件傳遞能力並擴展個人化銷售通訊。 這項新技術會自動管理電子郵件傳送時間，為[!DNL Exchange]和Gmail使用者建立順暢的體驗。 減少或避免使用協力廠商大量電子郵件傳送應用程式，並放心地從[!DNL Sales Connect]傳送您的所有電子郵件。

>[!NOTE]
>
>Beta現在提供電子郵件節流功能。 [了解更多](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

* **增強型銷售活動深入分析**：根據您銷售團隊先前的活動，擷取並啟用個人化參與。 新的屬性（例如「銷售電話錄音」連結、銷售促銷活動名稱和銷售電子郵件主旨）可用於Marketo Engage智慧清單。  這些活動可透過Marketo Engage REST API或大量匯出功能匯出和報告，並可在篩選器和觸發器上使用，作為智慧清單的額外限制。

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible][!DNL LinkedIn] Lead Gen Forms整合**：行銷人員現在可以對[!DNL LinkedIn]透過其Lead Gen Forms廣告單位擷取表單填寫時發生的轉換執行收入歸因。 這些見解可用於最佳化表單效能和付費媒體投資。 [!DNL LinkedIn] Lead Gen Forms是[!DNL LinkedIn]增長最快的付費媒體方案之一，這項新功能包含在我們與[!DNL Bizible]的現有[!DNL LinkedIn]廣告整合中。 
 
* **已改善Velocity儀表板**：我們已新增新的Velocity量度和儀表板篩選器，以取得更深入的見解。 此儀表板可供行銷人員用來瞭解逐階段銷售線索和機會速度，以及不同行銷和銷售參與形式的效率。

* **新同類群組瀑布歷程儀表板**：這可讓行銷人員檢視所選同類群組在傳統「需求瀑布」階段集中的進度，進而快速了解轉換率和隱含的階段轉換因果關係（依階段區分）。

## [!DNL Bizible]與Adobe Experience Cloud整合 {#bizible-integration-with-adobe-experience-cloud}

本節包含適用於已完成Adobe Identity Management系統(IMS)移轉的Bizible使用者的新功能。 如果您已移轉，您會在Adobe ID標籤下方的「[!DNL Bizible]設定」中看到新的Adobe ID。 所有帳戶皆應於2021年底前移轉。

* **[!DNL Bizible]與Adobe Privacy Service**&#x200B;的整合（2021年9月推出）： [!DNL Bizible]與Adobe Privacy Service的整合可跨Adobe Experience Cloud應用程式集中遵循關鍵資料隱私權法規（例如GDPR）。 您現在可以善用此服務，集中管理所有隱私權要求，以便在[!DNL Bizible]和其他Adobe產品中反映的變更要求。

* Adobe Unified Shell **上的**&#x200B;[!DNL Bizible]： [!DNL Bizible]採用Adobe Unified Shell後，使用者可擁有新功能，這些功能將出現在[!DNL Bizible]應用程式標題列中，並可更輕鬆存取支援資源及應用程式切換。 Adobe Unified Shell可協助在[!DNL Bizible]和其他Adobe Experience Cloud應用程式之間建立一致的體驗。

* **[!DNL Bizible]網域擁有權和自我管理**： [!DNL Bizible]使用者可運用Adobe Admin Console來管理他們要[!DNL Bizible]追蹤的網域。 這可為先前手動的流程帶來自助服務，並提供在Adobe Experience Cloud應用程式間管理網域所有權和追蹤的一致體驗。

## 公告 {#announcements}

* **更新至訂閱通用ID設定**：為了支援現有使用者即將整合的Marketo Engage和Adobe身分，所有Marketo Engage訂閱將在啟用通用ID支援中整合。 如需詳細資訊[，請參閱此處](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)。

**_產品發行網路研討會_**

[2021年8月Marketo Engage發行網路研討會](https://engage.marketo.com/August21_Release_Webinar.html)
