---
unique-page-id: 37357276
description: 發行說明 — 2020年6月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
source-git-commit: 6679e1e0bdb53d3f330c15415a5fbe38f61d28d2
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# 發行說明：』20年6月 {#release-notes-june}

』20年6月發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號(![](assets/yellow-star.png))表示的功能為付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每_** 季版本下列功能將於2020 **年6月5日發行**。

## 核心Marketo Engage {#core-marketo-engage}

* **[預測對象](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星號）](assets/yellow-star.png):全新Adobe Sensei提供的智慧清單和智慧行銷活動篩選器，可讓您為電子郵件、活動和網路研討會行銷方案建立AI支援的受眾區段。使用AI可協助您根據潛在客戶註冊事件、參加活動或取消訂閱的可能性來劃分受眾。 根據過去的計畫建立相似受眾，以有效複製先前的成功。 透過預測性目標追蹤來達成轉換目標，並取得建議，了解如何為事件方案調整您的對象區段。
* **批次電子郵件加速** ![（星號）](assets/yellow-star.png):增強我們的電子郵件行銷功能，可讓您每小時傳送最多300萬封批次電子郵件。我們已重新規劃批次行銷活動和電子郵件報表處理，以提升電子郵件方案和批次電子郵件行銷活動的效能。 這樣會縮短傳送的前置時間，並改善完成時間。 按照正常方式設定電子郵件傳送，不會增加複雜性。 此增強功能以產品附加元件的形式提供，其中也包含Delivery Services Launch Pack、電子郵件傳遞工具及多個專用IP位址。
* **[對象與Adobe Experience Cloud(AEC)整合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:全新Adobe Experience Cloud(AEC)整合，可讓您透過多個AEC應用程式同步來自Marketo Engage的已知銷售機會靜態清單，以增強現有計畫、解鎖新的使用案例，並協調多管道行銷活動。此整合包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **[方案成員自定義欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**:捕獲並利用關於方案成員的自定義欄位。在您的Marketo Engage表單中使用這些新欄位，在方案的成員清單中查看這些欄位，在智慧清單篩選器和觸發器中加以運用，並將它們納入新的智慧促銷活動流程動作中，以增強自動化和更精細的個人化。 您也可以透過UI和API匯入和匯出這些項目。 增強自訂資料物件和欄位功能。
* **說明方案成員**:檢索方案成員元資料，使您能夠使用REST API導入和導出方案成員自定義欄位資料。增強我們的API。
* **[在Microsoft Dynamics中建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**:根據Marketo Engage中捕獲的客戶行為，使用新的「流動操作」為Microsoft Dynamics內的銷售建立任務。增強我們原生的Microsoft Dynamics CRM整合。
* **取得清單資產API端點使用的表單**:擷取依賴表單的資產清單。增強我們的API。
* **透過API設定電子郵件前置詞**:啟用電子郵件首頁欄位的自動翻譯和本地化。增強我們的API。
* **影像和檔案快取**:我們正在從60秒的快取中提供影像和檔案資產，以增強Marketo Engage伺服器的穩定性。

## 帳戶型行銷 {#account-based-marketing}

![（星號）](assets/yellow-star.png)

* **新客戶發現正式提供**

   * 新客戶發現是對我們「客戶分析」功能的增強，它使您能夠根據AI支援的理想客戶配置檔案模型發現ABM策略的新目標客戶。 檢視、選取和匯入建議的新帳戶，以及其以AI為基礎的符合度和意圖資料指標。

<br> 

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

## Bizible {#bizible}

![（星號）](assets/yellow-star.png)

* **Marketo Engage計畫整合**:直接從Marketo Engage提取方案資料，在Bizible的歸因歷程中建立接觸點，以適當評分電子郵件和參與方案。增強我們的Marketo Engage整合。
* **Marketo Engage活動整合（測試版）**:將Marketo Engage活動資料直接匯入Bizible，以在客戶歷程和所有歸因模型中建立接觸點。範例包括銷售機會分數變更、有趣的時刻、電子郵件點按或任何自訂活動。 增強我們的Marketo Engage整合。
* **Bizible B2B客戶屬性整合(BETA)**:這是與Adobe Analytics的Adobe Experience Cloud整合，可讓您將選取的Bizible資料直接匯入Adobe Analytics，以便進行更深入的分析。例如，依公司名稱、帳戶屬性、CRM機會，以及Bizible歸因收入和漏斗階段所定義的高價值個人，以帳戶為基礎的網站流量和內容分析。
* **Bizible Discover篩選器和增強功能**:透過控制面板的管道、子管道、行銷活動和群體篩選來分析資料。透過更深入的屬性來增強資料可見性。 這是對Discover展示板的增強。
* **Microsoft Dynamics的活動同步**:將Microsoft Dynamics CRM活動帶入接觸點歷程，並追蹤與您的銷售機會或聯絡人相關聯的呼叫、約會或任務等事件，借此歸因銷售互動。增強我們的Microsoft Dynamics CRM整合。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

* **[適用於Salesforce CRM的前瞻分析控制面板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**:我們正在重新構想Sales Insight功能，同時提供即將進行之行銷活動和行銷活動的全新可見度，讓銷售者能夠根據客戶和潛在客戶的需求和興趣，提出更相關的建議。銷售商也可以在時間軸內檢視聯絡和帳戶活動，並輕鬆存取其他活動詳細資訊。 有關如何升級包[的更多詳細資訊，請參閱這裡](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)。

<br> 

## 公告 {#announcements}

* **ITP 2.1+ RTP更新**:由於Safari的Cookie原則有所變更，RTP Cookie在相同網域上跨工作階段追蹤使用者的能力，將會受到ITP限制，期限為1天或7天，視訪客使用的瀏覽器和瀏覽器版本而定。為此，我們正在實作新的網站服務，以允許透過HTTP回應以Set-Cookie標題設定RTP Cookie。 如需詳細資訊，請參閱[此處](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)。

* **批次促銷活動基礎架構變更**:今年剩餘時間內，我們將升級批次促銷活動服務。這將是無縫更新，不會影響正在進行的任何批次促銷活動，且不會導致行為變更。 不需要任何動作。 如需詳細資訊，請參閱[國家貼文](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)。

## 淘汰 {#deprecations}

* **[Munchkin關聯銷售線索](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:從Munchkin JS 159版開始，當叫用「關聯銷售機會」方法時，瀏覽器主控台將會記錄淘汰警告，指出該功能將在未來版本中移除。 完整淘汰時間表將於稍後宣佈。

**_產品發_** [行網路研討會觀](https://engage.marketo.com/June-Release-2020-On-Demand.html) 看』20年6月產品發行創新網路研討會的記錄。
