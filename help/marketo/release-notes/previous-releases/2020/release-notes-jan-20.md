---
unique-page-id: 37355534
description: 發行說明 — 2020年1月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年1月
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 發行說明：2020年1月 {#release-notes-jan}

2020年1月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號( ![（星形）](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將會發行於 **2020年1月17日**.

## 核心Marketo EngageAdobe應用程式 {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager資產選擇器](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md)：快速存取與您品牌一致的資產，並直接在Marketo Engage中使用AEM資產。 注意：雖然此功能同時適用於我們的Marketo Sky和傳統體驗，但管理功能可在我們的傳統體驗中找到。 您必須是AEM Assets的客戶，並擁有6.5版或更新版本。

>[!NOTE]
>
>目前，Firefox僅完全支援AEM資產選擇器。 Safari不支援此功能，且根據您的SameSite Cookie設定，此功能在最新版Chrome (v. 80)中可能無法運作。

* **Microsoft Dynamics — 即時同步銷售機會至CRM**：即時同步Marketo Engage和Microsoft Dynamics之間的潛在客戶與聯絡人。 建立銷售機會或聯絡人，並透過「將人員同步至Microsoft」流程動作立即在Microsoft Dynamics中檢視。
* **linkedIn潛在客戶Gen Forms其他欄位對應**：從LinkedIn Lead Gen Forms擷取銷售機會資料，針對銷售和行銷接觸點建立更相關的體驗。 將隱藏欄位、同意欄位和測試潛在客戶欄位提取到Marketo Engage中。
* **電子郵件範本相依性API**：取得取決於電子郵件範本的資產清單，以瞭解潛在變更的範圍，並解決對範本的相依性可以更快變更和刪除。
* **多執行個體管理增強功能**：使用訂閱的可捲動字母順序下拉式選單，快速導覽至您需要的執行個體。

## Account-Based Marketing {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **[新帳戶探索(BETA)](https://docs.marketo.com/x/WQA6Ag) ![（星形）](assets/yellow-star.png)**：使用帳戶分析，根據您的AI支援的理想客戶設定檔模型來探索ABM策略的全新目標帳戶。 檢視、選取和匯入建議的新帳戶，以及其以AI為基礎的配合與意圖資料指標，這些尚未存在於您的Marketo Engage銷售機會和帳戶資料庫中，以進行ABM目標定位。 立即可供符合帳戶分析客戶資格的客戶使用。

<br> 

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## Bizible {#bizible}

![（星形）](assets/yellow-star.png)

* **Marketo Engage銷售機會整合**：將銷售與行銷結合在一起，並透過跨Bizible和Marketo Engage的統一潛在客戶檢視。 透過此更新，Marketo Engage現在可以用作額外的銷售機會資料來源，因此您不再需要等待銷售機會與CRM同步以報告銷售機會產生。
* **探索增強功能**：利用根據客戶意見反應開發的增強功能，例如從圖磚和屬性向下展開至異動記錄、新增基本記錄計數和相應的單筆成本量度，以及新增/移除多個儀表板的儀表板篩選器，進一步瞭解在Bizible中探索儀表板。 您也會在登入時直接進入預設儀表板。

## Marketo Sky {#marketo-sky}

* [影像編輯](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio)：存取Adobe的編輯功能而無須離開Marketo Engage。 這項新功能可讓您直接在Design Studio中輕鬆增強、裁切及新增文字至影像。

## 銷售分析 {#sales-insight}

* **Salesforce閃電般的大量動作**：提升銷售效率，讓買家持續參與，能夠新增最多200個聯絡人/銷售機會至行銷活動，並透過Salesforce Lightning大量傳送Marketo Engage電子郵件。
* **Salesforce1的行動支援**：您現在可以在Salesforce1應用程式中，透過行動裝置存取所有Sales Insight功能，例如「有趣的時刻」和「網頁活動和電子郵件」。
* **UI增強功能**：更新介面，增強可讀性，且設計與Marketo Sky體驗一致。

## Sales Connect {#sales-connect}

* **格線元件**：使用新的網格自訂功能最佳化您的Sales Connect執行個體。 選擇要顯示的欄、搜尋欄、選取/取消選取所有欄，以及決定要在每個頁面上檢視多少資料列。
* **[內容鎖定](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**：透過全訂閱設定最大化品牌一致性，該設定可控制非管理員是否能夠建立和編輯範本和行銷活動。

>[!NOTE]
>
>* **不再使用TLS 1.0和1.1**：為了與Adobe的發行結構持續整合，我們將TLS 1.0和TLS 1.1的淘汰時間轉移至2020年1月13日。 可以找到更多詳細資訊 [此處](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **ITP 2.1+ Munchkin更新**：由於Safari的Cookie政策變更，Munchkin在同一網域上跨工作階段追蹤使用者的能力，將由ITP根據訪客使用的瀏覽器和瀏覽器版本限製為1或7天。 為此，我們正在實作新的Web服務，以允許透過HTTP回應以Set-Cookie標頭設定Munchkin Cookie。 如需如何實作此新服務的詳細資訊，請參閱 [此處](https://nation.marketo.com/docs/DOC-7351).

**_產品發行網路研討會_** [加入我們](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 太平洋時間3月3日上午11:00 /下午2:00舉辦產品團隊舉辦的即時網路研討會，並進一步瞭解此版本包含的功能。
