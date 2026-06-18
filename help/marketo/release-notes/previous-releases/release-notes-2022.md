---
title: 2022
description: 2022 - Marketo檔案 — 產品檔案
feature: Release Information
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 5247efff11566852d4c7271f1d212cc233593c19
workflow-type: tm+mt
source-wordcount: 4254
ht-degree: 6%

---

# 2022

## 2022 年 1 月 {#january}

2022年1月發行版本包含下列功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**

下列功能將於&#x200B;**2022年1月21日**&#x200B;開始發行，並在接下來的幾週內分階段推出每個功能（除非另有指定）。

## 次世代體驗

* **新一代體驗中的Screens已更新**：我們為新一代體驗提供額外的重新整理熒幕，透過切換開關提供更新的設計和可用性增強功能：

   * 在[!UICONTROL Design Studio]中的登陸頁面資產詳細資訊
   * 在[!UICONTROL Marketing Activities]中的登陸頁面資產詳細資訊

## [!DNL Microsoft Dynamics]整合 {#microsoft-dynamics-integration}

* **同步多重選取選項集欄位型別一般可使用**：同步處理來自[!DNL Microsoft Dynamics]的多重選取選項集欄位型別，以便在智慧列示和智慧行銷活動中運用，以更精細地鎖定受眾。 例如：相關主題/產品、偏好的通訊模式等。 此新同步處理適用於[!DNL Microsoft Dynamics] 9.X版（包括Dynamics 365 Online）。

* **[!DNL Microsoft Dynamics 365 Online]**&#x200B;的伺服器對伺服器驗證：為了提高安全性，我們現在將支援伺服器對伺服器(S2S)，作為Azure Active Directory上Marketo Engage同步處理使用者的額外驗證模式，以非互動式存取[!DNL Microsoft Dynamics 365 Online]。 這可讓您採用多重驗證，因為所有驗證和登入都將以OAuth為基礎（只有使用者端ID和使用者端密碼）。

>[!NOTE]
>
>S2S模式是以「應用程式使用者」而非「授權使用者」為基礎，因此可節省額外授權的使用。

## 管理 {#administration}

* **[表單驗證規則](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：維護資料庫的健全狀態，能夠封鎖有問題或不需要的電子郵件網域不提交Marketo Engage表單。 「全域表單驗證規則」面板可讓管理員定義封鎖清單，或啟用預先定義的免費消費者網域清單，以封鎖表單。

* **[登陸頁面標頭安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理員可以管理其登陸頁面網域上的嚴格傳輸安全性和X-Frame Options標頭，以強制執行強大的安全性要求。

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## AEP Marketo Engage目的地聯結器 — 建立全新銷售機會 {#aep-marketo-engage-destination-connector}

同時使用Adobe Experience Platform (AEP)的Marketo Engage客戶可透過Marketo Engage目的地聯結器，將全新人員記錄從AEP推送至AEP，讓資料庫發揮最大效用。 從AEP傳送對象區段至Marketo Engage時，區段內尚未存在於Marketo Engage資料庫[中的人員可自動新增至該資料庫](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## [!DNL Sales Insight]

![（星形）](assets/yellow-star.png)

[!DNL Salesforce] CRM **的**&#x200B;[!DNL Sales Insight]

* **適用於[!UICONTROL Best Bets]**&#x200B;的新型別欄：賣家將透過標籤為「型別」的新欄取得更快的深入分析，以區分[!UICONTROL Best Bets]頁面上的潛在客戶與聯絡人。

* **[!DNL Salesforce]Platform API更新**：為回應[!DNL Salesforce]淘汰[!DNL Salesforce] Platform API 21.0到30.0版，[!DNL Sales Insight]套件已更新為最新的API。

* **已更新品牌**：正在更新所有[!DNL Sales Insight]頁面，以符合Adobe品牌。

[!DNL Microsoft Dynamics]&#x200B;**的**&#x200B;[!DNL Sales Insight]

* **已更新帳戶配置**：賣家可取得熱門活動的集體檢視，例如：電子郵件活動、網路活動、有趣的時刻，以及帳戶內所有連絡人的分數變更。

## [!DNL Sales Connect]

![（星形）](assets/yellow-star.png)

* **通話結果和原因**：透過全新、完全可自訂的通話結果和通話原因選項，更詳細地瞭解及追蹤您的銷售團隊的出站工作。 除了這些新欄位之外，我們還將推出新的控管以強制進行來電原因和結果選擇、新的控管以啟用或停用來電原因和結果，以及新的來電原因和來電結果[!DNL Salesforce]活動自訂欄位，以將資料記錄到[!DNL Salesforce]。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)瞭解更多資訊。

* **[!DNL Salesforce]活動詳細資料自訂**：當銷售活動從[!DNL Sales Connect]登入[!DNL Salesforce]時，自訂要新增哪些資訊到[!DNL Salesforce]任務主題欄位，以在[!DNL Salesforce]中擷取更多銷售活動和任務資料。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)瞭解更多資訊。

## 公告

* **棄用Marketo Sky**：三月起，我們將不再提供Marketo Sky，因為我們的資源著重於提供新一代的使用者體驗。 為了維持對當今Marketo Sky專屬功能的存取權，我們在3月將資產到期和智慧型行銷活動優先順序覆寫帶入主流體驗。 [按一下這裡](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)瞭解更多資訊。

* **表單端點淘汰**：Marketo Engage表單將拒絕不支援的leadCapture/save2端點程式化表單POST。 [按一下這裡](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)瞭解更多資訊。

* **在[邀請使用者]對話方塊中登入**： 3月起，將棄用現有的選擇性功能[在邀請使用者對話方塊中登入]。 即將推出的Adobe Identity Management系統整合需要通用ID功能，而此功能已在2021年8月對所有訂閱啟用「[!UICONTROL Login in Invite User Dialog]」功能。 淘汰後，Marketo Engage將僅強制訂閱內每個電子郵件地址關聯一名使用者。

**Marketo Engage網域 — [!DNL Sales Insight]設定**：對於未布建SSL憑證和https://的Marketo Engage網域，呼叫將失敗並出現SSL交握錯誤。 因此，這些網域將被淘汰。 因此，具有指向這些網域中任何網域之舊設定的[!DNL Sales Insight]使用者可能在其Lead、Contact、Account、Opportunity Panels或Marketo Global頁面上遇到系統圖說文字錯誤。 如果您發生這個錯誤，建議您在[!DNL Salesforce]更新[Marketo Engage設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)。 您只需要更新在檔案的「[!DNL Marketo Sales Insight]設定」區段中醒目提示的Marketo Engage認證。

**_產品發行網路研討會_**

[2022年1月Marketo Engage版本網路研討會](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## 2022 年 3 月 {#march}

2022年3月發行版本包含下列功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**

下列功能將於&#x200B;**2022年3月11日**&#x200B;開始發行，並在接下來的幾週內分階段推出每個功能（除非另有指定）。

## 跨頻道協調

* **[!DNL Dynamic Chat]**：透過主動式、主動式和1:1個人化對話將目標同時鎖定於銷售機會和帳戶，在您的網站上最大化每個商機。 [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}可讓Marketo Engage使用者開始運用聊天，作為B2B行銷和銷售使用案例整合式跨管道體驗的關鍵部分。 功能包括：直接在聊天中預約會議、潛在客戶路由、入門範本、建立拖放式交談等等。 Dynamic Chat包含在所有Marketo Engage套件中，並將於今年推出給所有Marketo Engage使用者。

* **電子郵件機器人活動篩選增強功能**：作為先前發行之[電子郵件機器人活動篩選](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}功能的增強功能，您現在可以選擇加入識別為機器人的記錄活動。 然後，您可以根據識別為機器人正在執行的活動來篩選及觸發動作。

## 次世代體驗

* **新一代體驗中的Screens已更新**：我們為新一代體驗提供額外的重新整理熒幕，透過切換開關提供更新的設計和可用性增強功能：

   * [!UICONTROL Design Studio]中的表單清單檢視（包括新的大量動作）

* **匯入方案工作流程更新**：正在新一代體驗中傳遞匯入方案工作流程，其中包含更新的設計和可用性增強功能。 這將是一個自動變更，不需要切換開關。

* **新一代體驗切換開關的管理員控制**：以適合您的使用者的方式管理新一代體驗的推出，同時管理員能夠選取哪些使用者型別可以存取切換開關。

## 體驗自動化

* **自助服務流程步驟(Beta)**：擴充Marketo Engage與您棧疊其他部分之間的連線，並有能力編寫自訂的流程步驟以用於Smart Campaigns。 Marketo使用者和合作夥伴均可運用此功能，允許在批次和可執行的行銷活動中使用外部Web服務，而非Webhook，後者只能用於觸發行銷活動。

* **資產有效期**：保持對時效性資產和行銷活動的控制，並能夠在傳統使用者體驗中的指定日期和時間排程其自動停用。

* **智慧型行銷活動優先順序覆寫**：確保高優先順序觸發智慧型行銷活動會儘快執行，並有能力覆寫標準行銷活動優先順序排名。 低優先順序觸發器智慧型行銷活動也可以降低優先順序，以釋出處理資源給其他高優先順序的工作。

## API增強功能

* **傳回停用電子郵件的開啟追蹤狀態**：允許透過API讀取電子郵件的開啟追蹤狀態
* **從電子郵件擷取動態內容主旨列**：可讓行銷人員在BI工具中執行動態主旨列分析
* **方案成員自訂欄位CRUD**：可讓行銷人員以程式設計方式建立方案成員自訂欄位
* **大量自訂物件匯出已更新於Filter**：可讓行銷人員以程式設計方式同步自訂物件
* **公開電子郵件程式的Head Start設定**：可讓行銷人員透過API設定電子郵件程式的Head Start
* **選擇性方案標籤更新**：可讓行銷人員推播選擇性標籤更新，而不需同時推播所有標籤
* **大量活動擷取actionResult欄位**：可讓行銷人員識別哪些活動被略過或失敗

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## [!DNL Bizible] {#bizible}

![（星形）](assets/yellow-star.png)

* **BI範本**： [!DNL Bizible]現在將提供Tableau和Power BI的可下載基礎報告成品和範例報告，以便快速開發針對您特定業務需求量身打造的自訂報告。

## [!DNL Sales Connect]

![（星形）](assets/yellow-star.png)

* **電子郵件連線節流(GA)**：電子郵件連線節流可讓[!DNL Sales Connect]管理員設定使用Gmail或[!DNL Exchange]作為傳遞通道時的電子郵件傳送速率，讓電子郵件傳送給傳遞通道提供者的速率不超過強制的限制。

## 公告

* **棄用Marketo Sky**：三月起，我們將不再提供Marketo Sky，因為我們的資源著重於提供新一代的使用者體驗。 為了維持目前Marketo Sky專屬功能的存取權，我們將「資產有效期」和「智慧型行銷活動優先順序覆寫」引入傳統體驗。 [按一下這裡](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)瞭解更多資訊。

**_產品發行網路研討會_**

[2022年3月和5月Marketo Engage版本網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## 2022 年 5 月 {#may}

以下是2022年5月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**

下列功能將於2022年5月6日&#x200B;**開始發行**，並在接下來的幾週內分階段推出剩餘功能（除非另有指定）。

## 原生CRM整合 {#native-crm-integration}

**[原生Veeva CRM整合](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （可用性限制）**：透過原生整合，在Veeva CRM與Marketo Engage之間同步活動，以改善與醫療專業人員的互動。 此整合可讓行銷人員為醫療保健專業人員建立更個人化且順暢的跨管道體驗。 如果您有興趣參與，請聯絡您的客戶成功案例經理。

## 跨頻道協調

**[!DNL Dynamic Chat]**&#x200B;的聊天機器人事件：利用網頁訪客的更詳細行為資料，例如頁面逗留時間、網站逗留時間和頁面捲動百分比，以定義應顯示聊天對話方塊的時間。

**為[!DNL Dynamic Chat]**&#x200B;內嵌PDF：將PDF內嵌到聊天對話方塊中，並透過參與活動追蹤來測量內容效能，藉此提高參與度和共用有意義的內容。

**延伸語言支援[!DNL Dynamic Chat]**： [!DNL Dynamic Chat]使用者介面現在也提供法文、德文、日文、葡萄牙文和西班牙文版本。 也可以用這些語言設定聊天對話方塊。

**排除[!DNL Dynamic Chat]**&#x200B;的URL：控制您的網頁[!DNL Dynamic Chat]中哪些網頁會顯示，並能夠將特定URL從鎖定目標條件中排除。

**[電子郵件機器人活動篩選增強功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：除了現有的IAB清單比對識別之外，還能根據隱藏連結使用者代理程式或IP和近似程度模式來識別機器人行為，繼續保護資料庫的健全狀態。 檢視機器人活動統計資料，以瞭解每種型別識別的機器人活動數目。

**[電子郵件追蹤連結的STS標頭](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：符合安全性最佳實務，能夠套用Secure Transport Security標頭，以確保追蹤連結的流量一律安全。

## 次世代體驗

**切換切換預設為新一代體驗**：切換切換切換將在所有可用熒幕中預設為新體驗，讓使用者更容易發現更新的設計和可用性增強功能。

**已更新下一代體驗中的畫面**：

我們在[!UICONTROL Design Studio]內提供新一代體驗的電子郵件範本詳細資料檢視，提供更新的設計和可用性增強功能，可透過切換開關存取。

## 體驗自動化

**自助服務流程步驟（繼續測試版）**：擴充Marketo Engage與您棧疊其他部分之間的連線，並有能力編寫自訂流程步驟以用於Smart Campaigns。 Marketo Engage使用者和合作夥伴均可運用此功能，允許在觸發、批次和可執行的行銷活動中使用外部Web服務（相較於只能用於觸發行銷活動的Webhook）。

## API增強功能

* **已啟用CRM之訂閱的擴充API存取**：我們正在擴充已啟用CRM同步處理之訂閱的API存取，以允許使用者從Marketo Engage擷取公司、商機和銷售人員。
* **在Forms中支援「隱藏」資料型別**：提供透過API管理隱藏表單欄位的功能。
* **透過Rules支援isNot表單的多重比較值**：根據其他欄位的值是否不是指定清單中的值之一來管理表單欄位的可見度。
* **允許分別設定選取清單中的顯示值和提交值**：分別設定欄位中的顯示值和提交值。 例如，顯示飯店的名稱，但將內部ID提交至後端。
* **允許在建立或更新電子郵件時停用開啟追蹤的設定**：建立已停用開啟追蹤的電子郵件。

## 公告

**電子郵件驗證與唯一性**：從4月開始，將開始推出電子郵件驗證。 此時，Marketo Engage使用者電子郵件地址需要驗證和唯一性（這不適用於僅限API的使用者）。 目錄服務已驗證的使用者會在訂閱啟用電子郵件驗證時，自動驗證其電子郵件。

使用&quot;[!UICONTROL Login in Invite User Dialog]&quot;功能訂閱的電子郵件驗證，或是單一電子郵件與多位使用者相關聯的訂閱，將會與5月的發行保持一致。 若訂閱擁有與多位使用者相關聯的單一電子郵件，則會啟用電子郵件驗證，並將要求這些使用者解決衝突並使用每位使用者的唯一電子郵件。 啟用「在邀請使用者對話方塊中登入」功能時，透過此功能受邀的使用者將需要唯一的電子郵件地址。 對於透過此功能邀請的僅API使用者，電子郵件地址不需要是唯一的。

**封存資料夾行為變更**：在此版本中，樹狀內容功能表中將不再提供在封存資料夾中建立新資產的功能。 將會為所有資產隱藏用來建立新資產的功能表選項。 [若要了解更多資訊，請參閱此處](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}。

**_產品發行網路研討會_**

[2022年3月和5月Marketo Engage版本網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## 2022 年 6 月 {#june}

下方提供2022年6月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

下列功能將於&#x200B;**2022年6月24日**&#x200B;開始發行，並會在後續幾週內分階段推出剩餘功能（除非另有指定）。

## 行銷資料環境

* **公開自訂物件的CreatedAt/UpdatedAt欄位**：讓您能夠在「人員詳細資料」畫面中檢查這些欄位，以取得額外的insight。

## 跨頻道協調

* **改善[!DNL Dynamic Chat]**&#x200B;的串流Designer可用性：無需拖放，即可直接從Designer串流畫布新增卡片。 [!DNL Dynamic Chat]介面也已經過改良，以提供更清楚的個別卡片內容可見度。

* **[!DNL Dynamic Chat]**&#x200B;的進階約會路由規則： [!DNL Dynamic Chat]可提供更多目標約會路由的選項。 指定應根據Marketo Engage屬性路由哪些代理程式約會，確保將銷售機會路由至適當的代理程式。

* **[!DNL Dynamic Chat]**&#x200B;的進階對話方塊報告：使用參與和轉換量度的全新資料視覺效果，更詳細地檢視[!DNL Dynamic Chat]行銷活動的績效。

* **取消同步處理[!DNL Dynamic Chat]**&#x200B;未使用的Marketo Engage屬性：取消同步處理未使用的[!DNL Dynamic Chat]訂閱中的Marketo Engage屬性，協助您進行資料清理，並視需要同步替代屬性。

## 次世代體驗

**新的切換切換檢視**：以下檢視現在可在新一代體驗中使用：

* [電子郵件詳細資料視圖](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [電子郵件清單視圖](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 體驗自動化

* **全域表單欄位驗證規則排除**：從全域表單驗證規則中排除特定表單，以便訂閱中心和其他重要業務工作流程可以接受所有值。

* **自助服務流程步驟**：擴充Marketo Engage與您棧疊其他部分之間的連線，並有能力編寫自訂的流程步驟以用於Smart Campaigns。 Marketo Engage使用者和合作夥伴均可運用此功能，在「觸發器」、「批次」和「可執行促銷活動」中使用外部Web服務，而非Webhook，後者只能用於「觸發促銷活動」。

* **Munchkin通訊協定無關連結追蹤**：透過Munchkin延伸對`tel`和`mailto`連結追蹤的支援，以追蹤擴展的網頁行為集。

* **適用於Webhook的其他HTTP方法**：將PUT、PATCH和DELETE指定為與Web服務互動的請求型別。

## [!DNL Sales Insight]

![（星形）](assets/yellow-star.png)

* 在&#x200B;[!DNL Salesforce]&#x200B;**中設定的**&#x200B;[!DNL Sales Insight]&#x200B;許可權：管理員可以透過Marketo App許可權集（屬於[!DNL Sales Insight] [!DNL Salesforce]套件的一部分）提供[!DNL Sales Insight]存取權給使用者層級的有限人員集合，而非設定檔層級。

* **我的Marketo動態磚更新 — [!DNL Sales Insight]動作**： Marketo管理員（以及他們指定的使用者）現在可以透過位於「我的Marketo」頁面上的新[!DNL Sales Insight]動作動態磚，快速導覽至他們的[!DNL Sales Insight]動作執行個體。

## [!DNL Sales Connect]

![（星形）](assets/yellow-star.png)

* **[!DNL Salesforce]API更新**：隨著[!DNL Salesforce]夏季&#39;22的發行，[!DNL Salesforce]將不再支援API舊版21-30。 透過此Marketo Engage版本，使用舊版API的所有[!DNL Sales Connect]請求都已更新，以保持在支援的版本中。 如需[!DNL Salesforce] API淘汰計畫的完整詳細資料，請按一下[這裡](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}。

## API增強功能

* **大量程式成員擷取API的新篩選功能**：依程式成員資格狀態、updatedAt、cadence或用完的內容進行篩選，以精簡擷取的資料集。

* **大量程式成員擷取API改善**：在建立工作期間指定最多10個程式以改善輸送量。

## 公告

* **Forms淘汰 — Forms 1.0、銷售機會擷取/儲存端點，以及無指令碼版本的forms**：對Forms 1.0資產的支援將於2022年10月前從Marketo Engage中完全移除。 所有現有的Forms 1.0資產都將停止運作。 Marketo Engage表單將需要JavaScript才能載入登陸頁面和網站。

**_產品發行網路研討會_**

[2022年6月和8月Marketo Engage版本網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## 2022 年 8 月 {#august}

下方提供2022年8月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

下列功能於&#x200B;**2022年8月26日**&#x200B;開始分階段推出。

## 跨頻道協調

* 一次啟用/停用[!DNL Dynamic Chat]的所有已發佈對話方塊**：按一下按鈕，一次從設定頁面全域啟用/停用所有已發佈對話方塊。

* **[!DNL Dynamic Chat]**&#x200B;的自訂頭像：上傳自訂聊天機器人頭像，以便針對您的品牌進行個人化。

* **[!DNL Dynamic Chat]**&#x200B;的聊天記錄：檢視每個交談的聊天記錄，以深入瞭解insight每個網頁訪客感興趣的內容。

## 次世代體驗

* **Adobe品牌化**：更新了編輯的外觀和風格，以及具有新Adobe Experience Cloud品牌化的個人詳細資料頁面。

* **在移動對話方塊中顯示目的地資料夾的資料夾階層**：檢視每個資料夾的資料夾階層可讓移動資產更容易，並降低將資產放入錯誤資料夾的可能性。

* **[新一代體驗中的Screens已更新](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}**：我們為新一代體驗提供額外的重新整理熒幕，透過切換開關提供更新的設計和可用性增強功能：

   * 程式碼片段詳細資料
   * 「影像和檔案」詳細資料

>[!NOTE]
>
>在行銷活動中將資產移至方案中的資料夾為例外情況。 此移動動作不會顯示資料夾階層，因為程式中的資料夾名稱不能重複。

## 體驗自動化

* **[自助服務流程步驟 — 程式匯入增強功能](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**：已改善對匯入具有自訂流程步驟之程式的支援，您現在可以使用相同服務提供者的多個執行個體，以及匯入具有與這些服務提供者相容之流程步驟的程式。

* **[!DNL Munchkin]— 擴充的連結追蹤**：透過Munchkin擴充對`tel`和`mailto`連結的追蹤支援，以追蹤擴充的網頁行為集。

* **Webhook自訂標題可見性**： Webhook自訂標題現在顯示在[!UICONTROL Admin] > [!UICONTROL Webhooks]索引標籤中，以便更佳的可見性。

* **CAPTCHA**：使用reCAPTCHA v3[&#128279;](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}評估表單提交的有效性以評分傳入的表單流量。 建立行銷工作流程，以自動排除、隔離或刪除可疑的機器人流量。

* **核准表單的許可權**：新許可權，可控制哪些設計人員可核准與其他[!UICONTROL Design Studio]資產一致的表單變更。 這可以防止其他設計人員在沒有其他具有核准許可權的人員審閱表單的情況下，將變更推送至表單。

* **永遠在匿名合併後執行促銷活動重播**：匿名潛在客戶合併會在促銷活動重播之前發生，因此自訂欄位篩選器在匿名促銷活動重播完成時會可靠地運作。

## 行銷資料環境

* **修正自訂物件&quot;[!UICONTROL Used By]&quot;欄位的UI截斷**：現在更容易識別「使用中」的自訂物件欄位，因此您可以在必要時從自訂物件中刪除欄位。

## API增強功能

* **大量程式成員擷取API的新篩選功能**：依程式成員資格狀態、updatedAt、cadence或用完的內容進行篩選，以精簡擷取的資料集。

## [!DNL Sales Insight]

![（星形）](assets/yellow-star.png)

* **[[!DNL Sales Insight] 與 [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**&#x200B;整合：檢視[!DNL Sales Insight]面板中[!DNL Dynamic Chat]的活動，並將這個新的資料點用於您的潛在客戶工作。

## 公告

**_產品發行網路研討會_**

[2022年6月和8月Marketo Engage版本網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## 2022 年 10 月 {#october}

下方提供2022年10月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2022年10月14日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。 請檢視每個功能下方的狀態。

### 行銷資料環境

</br>

* **程式成員自訂欄位同步**：能夠雙向同步程式成員擷取的可延伸欄位（例如，在活動註冊期間與會者偏好設定，例如食物、工作階段、曲目等） Salesforce中的促銷活動成員欄位。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">方案成員自訂欄位同步</a></td>
  </tr>
  </tbody>
</table>

* **Adobe Privacy Service整合**：與Privacy Service協調，自動遵守Experience Cloud產品的資料隱私權法規。 目前，此服務僅適用於已上線Adobe Identity Management系統的Marketo Engage客戶。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### 次世代體驗

</br>

* **新一代體驗中的Screens已更新**：我們為新一代體驗提供額外的重新整理熒幕，透過切換開關提供更新的設計和可用性增強功能：

   * 登陸頁面範本詳細資料
   * 電子郵件範本清單

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">切換按鈕</a></td>
  </tr>
  </tbody>
</table>

* **電子郵件範本詳細資料中的索引標籤使用的增強功能**：在新體驗中，您會看到與使用電子郵件範本的資產相關的其他資訊，包括資產狀態、上次修改時間和上次修改者。 您也可以搜尋、排序及篩選資產使用的清單。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td>不適用</td>
  </tr>
  </tbody>
</table>

* **報表資產篩選模式**：報表組態模式的新設計，在組態功能表中顯示新的資產樹狀結構，以及建立和修改日期的篩選器。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td>不適用</td>
  </tr>
  </tbody>
</table>

### API增強功能

</br>

* **大量銷售機會匯入：銷售人員關聯**：與銷售機會REST API的同等性，可在大量銷售機會匯入程式期間將銷售機會與銷售人員關聯，減少所需的複雜度和API呼叫數。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">大量潛在客戶匯入</a></td>
  </tr>
  </tbody>
</table>

### 銷售Insight

</br>

![（星形）](assets/yellow-star.png)

* **銷售Insight與Dynamic Chat整合**： Insights Dashboard現在包含Smart Grid中的Dynamic Chat活動以及每週摘要和詳細資訊卡。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Dynamic Chat 整合</a></td>
  </tr>
  </tbody>
</table>

## 敏捷發行功能

以下功能遵循敏捷格式，並在標準發行日期之前或之後的各種日期發行。 請檢視每個功能下方的狀態。

* **自動排列Dynamic Chat的對話方塊資料流**：透過「自動排列」按一下按鈕，將畫布上的所有內容組織成簡潔且易於閱讀的格式，以改善您擁擠的對話方塊畫布。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">串流Designer圖示</a></td>
  </tr>
  </tbody>
</table>

* **Dynamic Chat的會議連結**：在傳送給訪客的每個行事曆邀請中，自動包含Google和Outlook的「團隊」或「會議」連結的選項。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">行事曆</a></td>
  </tr>
  </tbody>
</table>

* **支援Dynamic Chat的其他資料型別**：三種新資料型別（布林值、整數、浮點數）可讓您在Dynamic Chat中運用更多現有的Marketo Engage欄位，例如根據分數鎖定目標或詢問訪客是/否問題。

<table>
  <tr>
   <td><b>狀態</b></td>
   <td><b>文件更新</b></td>
  </tr>
  <tr>
   <td>已發行</td>
   <td>不適用</td>
  </tr>
  </tbody>
</table>

## 公告

* **Forms 1.0**： Forms 1.0將於10月發行版本中淘汰。 Forms 1.0資產無法再將資料提交至Marketo Engage，若嘗試將傳回錯誤。

* **無指令碼Forms**：在瀏覽器中停用Javascript時，Forms將不再運作。 提交表單需要啟用Javascript。
