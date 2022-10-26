---
unique-page-id: 37355534
description: 發行說明 — 2020年1月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年1月
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
source-git-commit: 12f45e694dccf1d9e51343b5eb9d743a8c513c1f
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 發行說明：2020年1月 {#release-notes-jan}

』20年1月發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號表示的特徵( ![（星號）](assets/yellow-star.png))是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_**

下列功能將於 **2020年1月17日**.

## 核心Marketo EngageAdobe應用程式 {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager Asset Selector](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md):透過直接在Marketo Engage中提供的AEM資產，快速存取與您品牌相符的資產。 注意：雖然我們的Marketo Sky和傳統體驗都提供此功能，但您可以在傳統體驗中找到管理功能。 您必須是AEM Assets的客戶，且有6.5版或更新版本。

>[!NOTE]
>
>目前，AEM Asset Selector僅完全支援Firefox。 Safari不支援，且視您的SameSite Cookie設定而定，在最新版Chrome(v. 80)中可能無法運作。

* **Microsoft Dynamics — 即時同步引導至CRM**:Marketo Engage和Microsoft Dynamics之間銷售機會和聯絡人的即時同步。 使用「將人員同步至Microsoft」流程動作，立即建立銷售機會或聯絡人，並在Microsoft Dynamics中查看他們。
* **linkedIn Lead Gen Forms其他欄位對應**:從LinkedIn Lead Gen Forms擷取銷售機會資料，為銷售和行銷接觸點建立更相關的體驗。 提取隱藏的欄位、同意欄位，測試將欄位帶入Marketo Engage。
* **電子郵件範本相依性API**:取得依賴電子郵件範本的資產清單，以了解潛在變更的範圍，並尋找範本的相依性，以便更快變更和刪除。
* **多執行個體管理增強功能**:使用訂閱的可捲動字母順序下拉式選單，快速導覽至您需要的執行個體。

## Account-Based Marketing {#account-based-marketing}

![（星號）](assets/yellow-star.png)

* **[新客戶發現（測試版）](https://docs.marketo.com/x/WQA6Ag) ![（星號）](assets/yellow-star.png)**:使用「帳戶配置檔案」，根據AI支援的理想客戶配置檔案模型，為您的ABM策略發現新的目標帳戶。 查看、選擇和導入建議的新帳戶，以及其基於AI的適切性和意圖資料指標，這些新帳戶在您的Marketo Engage線索和ABM目標定位帳戶資料庫中尚不存在。 可立即用於合格帳戶分析客戶。

<br> 

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

## Bizible {#bizible}

![（星號）](assets/yellow-star.png)

* **Marketo Engage銷售機會整合**:將銷售和行銷結合在一起，並統一檢視Bizible和Marketo Engage上的銷售機會。 透過此更新，Marketo Engage現在可作為額外的銷售機會資料來源使用，因此您不再需要等待銷售機會與CRM同步，即可報告銷售機會產生。
* **Discover增強功能**:透過客戶意見所開發的增強功能，讓Bizible的Discover展示板發揮更大效益，例如從圖磚和屬性深入鑽研至交易記錄、新增基本記錄計數和對應的每次成本量度，以及為多個控制面板新增/移除控制面板篩選器。 登入時也會直接帶您進入預設控制面板。

## Marketo Sky {#marketo-sky}

* [影像編輯](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio):存取Adobe的編輯功能，而不需離開Marketo Engage。 這項新功能可讓您直接在Design Studio中輕鬆執行增強、裁切和新增文字至影像等作業。

## Sales Insight {#sales-insight}

* **Salesforce閃電批量動作**:提高銷售效率，讓購買者能夠加入多達200個促銷活動聯絡人/銷售機會，並使用Salesforce Lightning大量傳送Marketo Engage電子郵件。
* **Salesforce1的行動支援**:您現在可以在Salesforce1應用程式中，對所有Sales Insight功能（例如「有趣的時刻」和Web活動與電子郵件）進行即時移動訪問。
* **UI增強功能**:更新介面，增強可讀性，並提供與Marketo Sky體驗一致的設計。

## Sales Connect {#sales-connect}

* **網格元件**:使用新的網格定制功能優化您的Sales Connect實例。 選擇要顯示的列、搜索列、選擇/取消選擇所有列，以及確定要在每個頁面上查看多少行資料。
* **[內容鎖定](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**:使用訂閱範圍設定，控制非管理員是否能建立及編輯範本和行銷活動，讓品牌與之保持最大一致。

>[!NOTE]
>
>* **不再使用TLS 1.0和1.1**:為了持續整合Adobe的發行結構，我們正在將TLS 1.0和TLS 1.1的淘汰功能轉移至2020年1月13日。 如需詳細資訊，請參閱 [此處](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **ITP 2.1+ Munchkin更新**:由於Safari的Cookie原則有所變更，ITP將限制Munchkin在相同網域上跨工作階段追蹤使用者的能力，根據訪客使用的瀏覽器和瀏覽器版本，這一限制為1或7天。 為此，我們實作了新的網站服務，允許透過HTTP回應以Set-Cookie標題設定Munchkin Cookie。 如需關於如何實作此新服務的詳細資訊，請參閱 [此處](https://nation.marketo.com/docs/DOC-7351).


**_產品發行網路研討會_** [加入我們](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3月3日上午11:00 PT /下午2:00 ET，由我們的產品團隊主持的線上網路研討會，深入了解此版本包含的功能。
