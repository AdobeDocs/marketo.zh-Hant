---
description: 發行說明 — 2022年6月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2022 年 6 月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 發行說明： 2022年6月 {#release-notes-june-22}

下方提供2022年6月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

下列功能將於&#x200B;**2022年6月24日**&#x200B;開始發行，並會在後續幾週內分階段推出剩餘功能（除非另有指定）。

## 行銷資料環境 {#marketing-data-environment}

* **公開自訂物件的CreatedAt/UpdatedAt欄位**：讓您能夠在「人員詳細資料」畫面中檢查這些欄位，以取得額外的insight。

## 跨頻道協調 {#cross-channel-orchestration}

* **改善[!DNL Dynamic Chat]**&#x200B;的串流Designer可用性：無需拖放，即可直接從Designer串流畫布新增卡片。 [!DNL Dynamic Chat]介面也已經過改良，以提供更清楚的個別卡片內容可見度。

* **[!DNL Dynamic Chat]**&#x200B;的進階約會路由規則： [!DNL Dynamic Chat]可提供更多目標約會路由的選項。 指定應根據Marketo Engage屬性路由哪些代理程式約會，確保將銷售機會路由至適當的代理程式。

* **[!DNL Dynamic Chat]**&#x200B;的進階對話方塊報告：使用參與和轉換量度的全新資料視覺效果，更詳細地檢視[!DNL Dynamic Chat]行銷活動的績效。

* **取消同步處理[!DNL Dynamic Chat]**&#x200B;未使用的Marketo Engage屬性：取消同步處理未使用的[!DNL Dynamic Chat]訂閱中的Marketo Engage屬性，協助您進行資料清理，並視需要同步替代屬性。

## 次世代體驗

**新的切換切換檢視**：以下檢視現在可在新一代體驗中使用：

* [電子郵件詳細資料檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [電子郵件清單檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 體驗自動化 {#experience-automation}

* **全域表單欄位驗證規則排除**：從全域表單驗證規則中排除特定表單，以便訂閱中心和其他重要業務工作流程可以接受所有值。

* **自助服務流程步驟**：擴充Marketo Engage與您棧疊其他部分之間的連線，並有能力編寫自訂的流程步驟以用於Smart Campaigns。 Marketo Engage使用者和合作夥伴均可運用此功能，在「觸發器」、「批次」和「可執行促銷活動」中使用外部Web服務，而非Webhook，後者只能用於「觸發促銷活動」。

* **Munchkin通訊協定無關連結追蹤**：透過Munchkin延伸對`tel`和`mailto`連結追蹤的支援，以追蹤擴展的網頁行為集。

* **適用於Webhook的其他HTTP方法**：將PUT、PATCH和DELETE指定為與Web服務互動的請求型別。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* 在&#x200B;[!DNL Salesforce]**中設定的**[!DNL Sales Insight]&#x200B;許可權：管理員可以透過Marketo App許可權集（屬於[!DNL Sales Insight] [!DNL Salesforce]套件的一部分）提供[!DNL Sales Insight]存取權給使用者層級的有限人員集合，而非設定檔層級。

* **我的Marketo動態磚更新 — [!DNL Sales Insight]動作**： Marketo管理員（以及他們指定的使用者）現在可以透過位於「我的Marketo」頁面上的新[!DNL Sales Insight]動作動態磚，快速導覽至他們的[!DNL Sales Insight]動作執行個體。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **[!DNL Salesforce]API更新**：隨著[!DNL Salesforce]夏季&#39;22的發行，[!DNL Salesforce]將不再支援API舊版21-30。 透過此Marketo Engage版本，使用舊版API的所有[!DNL Sales Connect]請求都已更新，以保持在支援的版本中。 如需[!DNL Salesforce] API淘汰計畫的完整詳細資料，請按一下[這裡](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}。

## API增強功能 {#api-enhancements}

* **大量程式成員擷取API的新篩選功能**：依程式成員資格狀態、updatedAt、cadence或用完的內容進行篩選，以精簡擷取的資料集。

* **大量程式成員擷取API改善**：在建立工作期間指定最多10個程式以改善輸送量。

## 公告 {#announcements}

* **Forms淘汰 — Forms 1.0、銷售機會擷取/儲存端點，以及無指令碼版本的forms**：對Forms 1.0資產的支援將於2022年10月前從Marketo Engage中完全移除。 所有現有的Forms 1.0資產都將停止運作。 Marketo Engage表單將需要JavaScript才能載入登陸頁面和網站。

**_產品發行網路研討會_**

[2022年6月和8月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
