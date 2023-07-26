---
unique-page-id: 37357276
description: 發行說明–2020年6月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# 發行說明： 2020年6月 {#release-notes-june}

2020年6月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_** 下列功能將會發行於 **2020年6月5日**.

## 核心Marketo Engage {#core-marketo-engage}

* **[預測對象](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星形）](assets/yellow-star.png)：由Adobe Sensei提供支援的新智慧列示和智慧行銷活動篩選器，可讓您為電子郵件、事件和網路研討會行銷方案建立AI支援的對象區段。 使用AI可協助您根據潛在客戶註冊事件、出席事件或取消訂閱的可能性來細分對象。 根據過去的計畫建立相似的受眾，以有效復寫先前的成功。 透過預測性目標追蹤達成轉換目標，並取得有關如何調整事件方案對象區段的建議。
* **批次電子郵件提升** ![（星形）](assets/yellow-star.png)：增強我們的電子郵件行銷功能，允許您每小時最多傳送300萬封批次電子郵件。 我們已重新架構批次行銷活動和電子郵件報告處理，以提升電子郵件程式和批次電子郵件行銷活動的效能。 這會縮短傳送的前置時間，並改善完成時間。 設定您的電子郵件傳送，如同您一般的作法，不會增加複雜性。 此增強功能可作為產品附加元件提供，其中也包含傳遞服務啟動套件、電子郵件傳遞工具和多個專用IP位址。
* **[對象與Adobe Experience Cloud (AEC)整合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：新的Adobe Experience Cloud (AEC)整合可讓您將Marketo Engage中已知銷售機會的靜態清單與多個AEC應用程式同步，以強化現有計畫、解鎖新使用案例，並協調多管道行銷活動。 此整合包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **[方案成員自訂欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**：擷取並利用有關方案成員的自訂欄位。 在Marketo Engage表單中使用這些新欄位、在方案的成員清單中檢視這些欄位、在智慧清單篩選器和觸發器中運用這些欄位，並將其納入新的智慧行銷活動流量動作中，以增強自動化和更精細的個人化。 您也可以透過UI和API匯入及匯出這些內容。 增強我們的自訂資料物件和欄位功能。
* **描述方案成員**：擷取方案成員中繼資料，讓您能夠使用REST API匯入和匯出方案成員自訂欄位資料。 增強API。
* **[在Microsoft Dynamics中建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**：根據Marketo Engage中擷取的客戶行為，使用新的流量動作在Microsoft Dynamics中建立銷售任務。 增強原生Microsoft Dynamics CRM整合功能。
* **取得清單資產API端點使用的表單**：擷取相依於表單的資產清單。 增強API。
* **透過API設定電子郵件預覽文字**：啟用電子郵件預覽文字欄位的自動翻譯和本地化。 增強API。
* **影像和檔案快取**：我們從60秒的快取中提供影像和檔案資產，以增強Marketo Engage伺服器的穩定性。

## Account-Based Marketing {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **新帳戶探索正式推出**

   * 新帳戶探索是我們的帳戶設定檔功能的增強功能，可讓您根據由AI支援的理想客戶設定檔模型，為ABM策略探索全新目標帳戶。 檢視、選取和匯入建議的新帳戶，以及其以AI為基礎的配合和意圖資料指標。

<br> 

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## Bizible {#bizible}

![（星形）](assets/yellow-star.png)

* **Marketo Engage計畫整合**：直接從Marketo Engage提取計畫資料以在Bizible中的歸因歷程中建立接觸點，以適當地點數電子郵件和參與計畫。 增強Marketo Engage整合功能。
* **Marketo Engage活動整合(BETA)**：將Marketo Engage活動資料直接引進Bizible，在客戶歷程和所有歸因模型中建立接觸點。 範例包括銷售機會分數變更、有趣的時刻、電子郵件點按或任何自訂活動。 增強Marketo Engage整合功能。
* **Bizible B2B客戶屬性整合(BETA)**：這是與Adobe Analytics的Adobe Experience Cloud整合，可讓您直接將選取的Bizible資料匯入Adobe Analytics，以進行更深入的分析。 範例包括依公司名稱、帳戶屬性、CRM商機以及Bizible歸因收入和漏斗階段定義的高價值個人的帳戶型網站流量和內容分析。
* **Bizible Discover篩選器和增強功能**：使用跨控制面板的管道、子管道、行銷活動和區段篩選器來分析您的資料。 使用更多向下鑽研屬性來強化資料的可見度。 這是我們Discover Boards的增強功能。
* **Microsoft Dynamics的活動同步**：將Microsoft Dynamics CRM活動引進接觸點歷程並追蹤事件（例如與潛在客戶或連絡人相關聯的電話、約會或工作），以歸因於銷售互動。 增強Microsoft Dynamics CRM整合功能。

## 銷售分析 {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[Salesforce CRM的深入分析控制面板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**：我們重新構想銷售深入分析功能，透過新的可見度來顯示即將推出的行銷活動和行銷活動，讓賣家能夠根據客戶和潛在客戶的需求和興趣，提供與客戶和潛在客戶更相關的建議。 賣家也可以在時間軸內檢視聯絡人和帳戶活動，並輕鬆存取其他活動細節。 尋找有關如何升級套件的詳細資訊 [此處](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## 公告 {#announcements}

* **ITP 2.1+ RTP更新**：由於Safari的Cookie原則有所變更，RTP Cookie在同一網域上跨工作階段追蹤使用者的能力，將由ITP根據訪客使用的瀏覽器和瀏覽器版本限製為1或7天。 為了解決這個問題，我們正在實作一項新的Web服務，以允許透過HTTP回應以Set-Cookie標頭來設定RTP Cookie。 可以找到更多資訊 [此處](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **批次促銷活動基礎結構變更**：我們將在今年餘下時間升級批次行銷活動服務。 這將是一次順暢的更新，不會影響任何正在進行的批次行銷活動，也不會導致行為變更。 不需要採取任何動作。 在此尋找更多詳細資料 [國家貼文](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## 淘汰 {#deprecations}

* **[Munchkin關聯銷售機會](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：自Munchkin JS版本159發行版本開始，呼叫Associate Lead方法時會從瀏覽器主控台記錄淘汰警告，這表示在未來發行版本中將移除該功能。  我們日後將公佈完整的淘汰排程。

**_產品發行網路研討會_** [觀看錄製](https://engage.marketo.com/June-Release-2020-On-Demand.html) 2020年6月產品發行創新網路研討會的。
