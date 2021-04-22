---
unique-page-id: 37357276
description: 發行說明- 2006年6月-Marketo文檔——產品文檔
title: 發行說明- 2002年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 0%

---

# 發行說明：6月20日{#release-notes-june}

6月20日發行包含下列功能。 查看您的Marketo版功能是否可用。

>[!AVAILABILITY]
>
>由星號(![(star)](assets/star-yellow.svg))表示的特徵可以是付費附加元件。 請連絡您的Marketo Engage代表以瞭解更多資訊。

**_每季_** 發行以下功能將於2020年6 **月5日發行**。

## 核心Marketo Engage{#core-marketo-engage}

* **[預測性觀眾](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星級）](assets/star-yellow.svg):全新的「智慧型清單」和「智慧型促銷活動」篩選器由Adobe Sensei提供支援，可讓您為電子郵件、活動和網路研討會行銷計畫建立人工智慧型受眾細分。使用人工智慧協助您根據潛在客源註冊活動、參加活動或取消訂閱的可能性來劃分受眾。 根據過去的計畫建立相似的受眾，以有效複製先前的成功。 運用預測性目標追蹤來達成轉換目標，並取得如何針對活動計畫調整受眾細分的建議。
* **批次電子郵件大幅** ![（星型）](assets/star-yellow.svg):增強我們的電子郵件行銷功能，讓您每小時傳送最多3百萬封批次電子郵件。我們已重新架構我們的批次促銷活動和電子郵件報表處理，以增強電子郵件程式和批次電子郵件促銷活動的效能。 如此可縮短傳送的前置時間，並改善完成時間。 設定您傳送的電子郵件，就像平常一樣，不會增加複雜性。 此增強功能可做為產品附加元件使用，其中也包含Delivery Services Launch Pack、電子郵件傳送工具和多個專用IP位址。
* **[與Adobe Experience Cloud(AEC)的受眾整合](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:全新的Adobe Experience Cloud(AEC)整合，可讓您將已知客源的靜態清單與多個AEC應用程式同步，以增強現有的方案、解除新的使用案例，並協調多通道宣傳。這一整合包括Adobe Analytics,Adobe Target,Adobe Experience Manager,Adobe Audience Manager和Adobe Advertising Cloud.
* **[方案成員自定義欄位](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**:擷取並運用方案會員的自訂欄位。在您的Marketo Engage表單中使用這些新欄位、在方案的成員清單中檢視這些欄位、在智慧型清單篩選器和觸發器中運用這些欄位，並將它們加入新的智慧型促銷活動流程動作，以增強自動化和更精細的個人化。 您也可以透過UI和API匯入和匯出這些檔案。 增強我們的自訂資料物件和欄位功能。
* **說明方案會員**:擷取方案會員中繼資料，讓您能夠使用REST API匯入和匯出方案會員自訂欄位資料。增強我們的API。
* **[在Microsoft Dynamics中建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**:根據在Marketo Engage中擷取的客戶行為，使用新的「流量動作」，在Microsoft Dynamics內建立銷售工作。增強我們原生的Microsoft Dynamics CRM整合。
* **取得清單資產API端點使用的表單**:擷取依賴表單的資產清單。增強我們的API。
* **透過API設定電子郵件預先標題**:啟用電子郵件標題欄位的自動轉譯和本地化。增強我們的API。
* **影像和檔案快取**:我們從60秒的快取中提供影像和檔案資產，以增強Marketo Engage伺服器的穩定性。

## 帳戶型行銷{#account-based-marketing}

![（星號）](assets/star-yellow.svg)

* **新帳戶發現已正式推出**

   * 「新客戶發現」是對「客戶分析」功能的增強，使您能夠根據基於人工智慧支援的理想客戶配置檔案模型發現ABM策略的新目標客戶。 檢視、選擇和匯入建議的新帳戶，以及其以AI為基礎的符合與意圖資料指標。

<br> 

**_整季發行_**

以下功能是非季度週期，將於未來數月內發佈。

## Bizible {#bizible}

![（星號）](assets/star-yellow.svg)

* **Marketo Engage方案整合**:直接從Marketo Engage擷取計畫資料，在Bizible的歸因歷程中建立觸點，以適當地為電子郵件和參與計畫提供信用。增強我們的Marketo Engage整合。
* **Marketo Engage活動整合(BETA)**:將Marketo Engage活動資料直接匯入Bizible，以建立客戶歷程和所有歸因模型的觸點。範例包括銷售機會分數變更、有趣時刻、電子郵件點按或任何自訂活動。 增強我們的Marketo Engage整合。
* **B2B客戶屬性整合(BETA)**:這是Adobe Experience Cloud與Adobe Analytics的整合，可讓您將精選的Bizible資料直接帶入Adobe Analytics，以進行更深入的分析。範例包括依公司名稱、帳戶屬性、CRM機會和高價值個人（如Bizbile歸因收入和漏斗階段所定義）進行帳戶型網站流量和內容分析。
* **奇怪的Discover篩選器和增強功能**:透過跨控制面板的渠道、子渠道、促銷活動和群體篩選，分析您的資料。使用更深入的屬性來增強資料可見度。 這是對Discover展示板的增強功能。
* **Microsoft Dynamics的活動同步**:將Microsoft Dynamics CRM活動引入接觸點歷程，並追蹤與您的潛在客戶或聯絡人相關的呼叫、約會或工作等事件，以歸因銷售互動。增強Microsoft Dynamics CRM整合。

## 銷售分析{#sales-insight}

![（星號）](assets/star-yellow.svg)

* **[Salesforce CRM的前瞻分析資料板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**:我們重新構思Sales Insight功能，並對即將到來的行銷活動和宣傳活動有新的洞察力，讓銷售者能夠根據客戶和潛在客戶的需求和興趣，提出更符合客戶和潛在客戶的建議。銷售者也可以在時間軸中檢視「連絡人」和「帳戶活動」，並輕鬆存取其他活動詳細資訊。 有關如何升級軟體包[的詳細資訊，請參閱](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md)。

<br> 

## 公告{#announcements}

* **ITP 2.1+ RTP更新**:由於Safari的Cookie原則有所變更，RTP Cookie在相同網域作業間追蹤使用者的能力將因訪客使用的瀏覽器和瀏覽器版本而受ITP限制為1或7天。為此，我們實作新的web services，允許透過HTTP回應以Set-Cookie標題來設定RTP Cookie。 如需詳細資訊，請至[這裡](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)。

* **批次促銷活動基礎架構變更**:我們將在今年剩餘時間升級我們的批次促銷活動服務。這將是順暢的更新，不會影響任何正在進行中的批次促銷活動，也不會導致行為變更。 不需要任何動作。 如需詳細資訊，請參閱[國家貼文](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)。

## 淘汰{#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:從159版Munchkin JS開始，當呼叫Associate Lead方法時，瀏覽器主控台會記錄取代警告，指出功能將在未來版本中移除。 完全淘汰的時間表將在稍後宣佈。

**_產品發行網_** [路研討會觀](https://engage.marketo.com/June-Release-2020-On-Demand.html) 看我們6月20日產品發行創新網路研討會的錄制。
