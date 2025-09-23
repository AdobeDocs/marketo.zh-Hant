---
unique-page-id: 37357276
description: 發行說明–2020年6月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 1%

---

# 發行說明：2020 年 6 月 {#release-notes-june}

2020年6月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))表示的功能是付費附加元件。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**&#x200B;下列功能將於&#x200B;**2020年6月5日**&#x200B;發行。

## 核心Marketo Engage {#core-marketo-engage}

* **[預測對象](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=zh-Hant#predictive-audiences)** ![(star)](assets/yellow-star.png)：由Adobe Sensei支援的新智慧列示和智慧行銷活動篩選器可讓您為電子郵件、事件和網路研討會行銷方案建立AI支援的對象區段。 使用AI可協助您根據潛在客戶註冊事件、出席事件或取消訂閱的可能性來細分對象。 根據過去的計畫建立相似的受眾，以有效復寫先前的成功。 透過預測性目標追蹤達成轉換目標，並取得有關如何調整事件方案對象區段的建議。
* **批次電子郵件提升** ![(star)](assets/yellow-star.png)：增強我們的電子郵件行銷功能，可讓您每小時最多傳送300萬封批次電子郵件。 我們已重新架構批次行銷活動和電子郵件報告處理，以提升電子郵件程式和批次電子郵件行銷活動的效能。 這會縮短傳送的前置時間，並改善完成時間。 設定您的電子郵件傳送，如同您一般的作法，不會增加複雜性。 此增強功能可作為產品附加元件提供，其中也包含傳遞服務啟動套件、電子郵件傳遞工具和多個專用IP位址。
* **[與Adobe Experience Cloud (AEC)的受眾整合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：全新的Adobe Experience Cloud (AEC)整合，可讓您將Marketo Engage的已知潛在客戶靜態清單與多個AEC應用程式同步，以強化現有計畫、解鎖新使用案例，以及協調多管道行銷活動。 此整合包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **[方案成員自訂欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**：擷取並利用方案成員的相關自訂欄位。 在Marketo Engage表單中使用這些新欄位、在方案的成員清單中檢視這些欄位、在智慧清單篩選器和觸發器中運用這些欄位，並將其納入新的智慧行銷活動流量動作中，以增強自動化和更精細的個人化。 您也可以透過UI和API匯入及匯出這些內容。 增強我們的自訂資料物件和欄位功能。
* **描述方案成員**：擷取方案成員中繼資料，讓您能夠使用REST API匯入和匯出方案成員自訂欄位資料。 增強API。
* **[在 [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**&#x200B;中建立任務：根據Marketo Engage中擷取的客戶行為，使用新的流程動作在[!DNL Microsoft Dynamics]中建立銷售任務。 增強我們原生[!DNL Microsoft Dynamics] CRM整合的功能。
* **取得清單資產API端點使用的表單**：擷取相依於表單的資產清單。 增強API。
* **透過API設定電子郵件預覽文字**：啟用電子郵件預覽文字欄位的自動翻譯和本地化。 增強API。
* **影像和檔案快取**：我們從60秒的快取中提供影像和檔案資產，以增強Marketo Engage伺服器的穩定性。

## Account-Based Marketing {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **一般可用的新帳戶探索**

   * 新帳戶探索是我們的帳戶設定檔功能的增強功能，可讓您根據由AI支援的理想客戶設定檔模型，為ABM策略探索全新目標帳戶。 檢視、選取和匯入建議的新帳戶，以及其以AI為基礎的配合和意圖資料指標。

<br>

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## [!DNL Bizible] {#bizible}

![（星形）](assets/yellow-star.png)

* **Marketo Engage程式整合**：直接從Marketo Engage提取程式資料，以在[!DNL Bizible]中建立歸因歷程中的接觸點，以適當地評價電子郵件和參與程式。 增強Marketo Engage整合功能。
* **Marketo Engage活動整合(BETA)**：將Marketo Engage活動資料直接匯入[!DNL Bizible]，以在客戶歷程和所有歸因模型中建立接觸點。 範例包括銷售機會分數變更、有趣的時刻、電子郵件點按或任何自訂活動。 增強Marketo Engage整合功能。
* **[!DNL Bizible]B2B客戶屬性整合(BETA)**：這是與Adobe Analytics的Adobe Experience Cloud整合，可讓您直接將選取的Bizible資料帶入Adobe Analytics，以進行更深入的分析。 範例包括以帳戶為基礎的網站流量，以及依公司名稱、帳戶屬性、CRM商機，以及[!DNL Bizible]歸因收入和漏斗階段定義的高價值個人的內容分析。
* **[!DNL Bizible]探索篩選器和增強功能**：使用跨控制面板的管道、子管道、行銷活動和區段篩選器來分析您的資料。 使用更多向下鑽研屬性來強化資料的可見度。 這是我們Discover Boards的增強功能。
* **[!DNL Microsoft Dynamics]**&#x200B;的活動同步：將[!DNL Microsoft Dynamics]個CRM活動帶入接觸點歷程並追蹤事件（例如與您潛在客戶或連絡人相關聯的電話、約會或工作），以屬性銷售互動。 增強我們的[!DNL Microsoft Dynamics] CRM整合。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[Salesforce CRM的深入分析儀表板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**：我們正在重新構想我們的[!DNL Sales Insight]功能，透過即將推出的行銷活動和行銷活動的全新可見度，讓賣家能夠根據客戶和潛在客戶的需求和興趣，提供更切合其需要的建議。 賣家也可以在時間軸內檢視聯絡人和帳戶活動，並輕鬆存取其他活動細節。 如需有關如何升級封裝的詳細資訊，請參閱[這裡](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)。

<br>

## 公告 {#announcements}

* **ITP 2.1+ RTP更新**：由於[!DNL Safari]的Cookie原則有所變更，RTP Cookie在同一個網域上跨工作階段追蹤使用者的能力，將由ITP根據訪客使用的瀏覽器和瀏覽器版本限製為1或7天。 為了解決這個問題，我們正在實作一項新的Web服務，以允許透過HTTP回應以Set-Cookie標頭來設定RTP Cookie。 在[這裡](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)可找到更多資訊。

* **批次行銷活動基礎結構變更**：我們將在今年剩餘的時間升級批次行銷活動服務。 這將是一次順暢的更新，不會影響任何正在進行的批次行銷活動，也不會導致行為變更。 不需要採取任何動作。 在此[國家貼文](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)中尋找更多詳細資料。

## 淘汰 {#deprecations}

* **[Munchkin關聯銷售機會](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：從[!DNL Munchkin] JS的159版開始，叫用Associate Lead方法時會從瀏覽器主控台記錄棄用警告，這表示在未來版本中會移除該功能。  我們日後將公佈完整的淘汰排程。

**_產品發行網路研討會_** [觀看我們2020年6月產品發行創新網路研討會的錄影](https://engage.marketo.com/June-Release-2020-On-Demand.html)。
