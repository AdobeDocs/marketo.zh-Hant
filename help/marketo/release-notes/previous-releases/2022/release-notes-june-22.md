---
description: 發行說明 — 2022年6月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年6月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 發行說明： 2022年6月 {#release-notes-june-22}

下方提供2022年6月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

下列功能將於&#x200B;**2022年6月24日**&#x200B;開始發行，並會在後續幾週內分階段推出剩餘功能（除非另有指定）。

## 行銷資料環境 {#marketing-data-environment}

* **公開自訂物件的CreatedAt/UpdatedAt欄位**：讓您能夠在「人員詳細資料」畫面中檢查這些欄位，以獲得更多深入分析。

## 跨頻道協調 {#cross-channel-orchestration}

* **改善Dynamic Chat的串流Designer可用性**：無需拖放，即可直接從Designer串流畫布新增卡片。 Dynamic Chat介面也已經過改良，以便提供更清楚的個別卡片內容顯示。

* **Dynamic Chat的進階約會路由規則**： Dynamic Chat提供更多目標約會路由的選項。 指定應根據Marketo Engage屬性路由哪些代理程式約會，確保將銷售機會路由至適當的代理程式。

* **Dynamic Chat的進階對話方塊報告**：使用參與和轉換量度的全新資料視覺效果，更詳細地檢視Dynamic Chat行銷活動的效能。

* **取消同步處理Dynamic Chat未使用的Marketo Engage屬性**：取消同步處理未使用的Dynamic Chat訂閱中的Marketo Engage屬性，協助您提升資料整潔度，並視需要同步處理其他屬性。

## 次世代體驗

**新的切換切換檢視**：以下檢視現在可在新一代體驗中使用：

* [電子郵件詳細資料檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [電子郵件清單檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 體驗自動化 {#experience-automation}

* **全域表單欄位驗證規則排除**：從全域表單驗證規則中排除特定表單，以便訂閱中心和其他重要業務工作流程可以接受所有值。

* **自助服務流程步驟**：擴充Marketo Engage與您棧疊其他部分之間的連線，能夠撰寫自訂的流程步驟以用於Smart Campaigns。 Marketo Engage使用者和合作夥伴均可運用此功能，在「觸發器」、「批次」和「可執行促銷活動」中使用外部Web服務，而非Webhook，後者只能用於「觸發促銷活動」。

* **Munchkin通訊協定不可知的連結追蹤**：使用Munchkin延伸對`tel`和`mailto`連結的追蹤支援，以追蹤擴充的網頁行為集。

* **適用於Webhook的其他HTTP方法**：將PUT、PATCH和DELETE指定為與Web服務互動的要求型別。

## 銷售分析 {#sales-insight}

![（星形）](assets/yellow-star.png)

* **Salesforce中的Sales Insight許可權集**：管理員可以透過Marketo App許可權集（屬於Sales Insight Salesforce套件的一部分），提供使用者層級上有限一組人員的Sales Insight存取權，而非設定檔層級。

* **我的Marketo動態磚更新 — Sales Insight動作**： Marketo管理員（以及他們指定的使用者）現在可以透過「我的Marketo」頁面上的新「Sales Insight動作」動態磚，快速導覽至他們的Sales Insight Actions執行個體。

## Sales Connect {#sales-connect}

![（星形）](assets/yellow-star.png)

* **Salesforce API更新**：隨著Salesforce Summer的22年發行版本，Salesforce將不再支援API舊版21-30。 透過此Marketo Engage版本，使用舊版API的所有Sales Connect請求都已更新，以保持在支援的版本中。 如需Salesforce API處分計畫的完整詳細資料，請按一下[這裡](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}。

## API增強功能 {#api-enhancements}

* **大量程式成員擷取API的新篩選功能**：依程式成員資格狀態、updatedAt、cadence或用完的內容進行篩選，以精簡擷取的資料集。

* **大量程式成員擷取API改善**：在建立工作期間指定最多10個程式以改善輸送量。

## 公告 {#announcements}

* **Forms淘汰 — Forms 1.0、銷售機會擷取/儲存端點，以及無指令碼版本的forms**：對Forms 1.0資產的支援將在2022年10月前從Marketo Engage中完全移除。 所有現有的Forms 1.0資產都將停止運作。 Marketo Engage表單將需要JavaScript在登陸頁面和網站上載入。

**_產品發行網路研討會_**

[2022年6月和8月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
