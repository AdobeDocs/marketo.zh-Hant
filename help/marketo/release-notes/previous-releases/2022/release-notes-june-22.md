---
description: 發行說明 — 2022年6月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年6月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# 發行說明： 2022年6月 {#release-notes-june-22}

下方提供2022年6月發行版本包含的所有功能。 檢視您的Adobe Marketo Engage版本，瞭解是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![星號](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

下列功能將開始發行： **2022年6月24日**，在接下來的幾週內分階段推出剩餘的功能（除非另有指定）。

## 行銷資料環境 {#marketing-data-environment}

* **公開自訂物件的CreatedAt/UpdatedAt欄位**：可讓您檢查「人員詳細資料」畫面中的這些欄位，以獲得更多深入分析。

## 跨頻道協調 {#cross-channel-orchestration}

* **改善Dynamic Chat的串流設計工具可用性**：直接從串流設計工具畫布新增卡片，無需拖放。 Dynamic Chat介面也經過改良，以便提供更清楚的個別卡片內容可見度。

* **Dynamic Chat的進階約會路由規則**：Dynamic Chat提供更多目標約會路由的選項。 指定應根據Marketo Engage屬性路由哪些代理程式約會，確保將潛在客戶路由至適當的代理程式。

* **Dynamic Chat的進階對話方塊報告**：使用參與和轉換量度的全新資料視覺效果，更詳細地檢視Dynamic Chat行銷活動的效能。

* **取消同步未使用的Dynamic ChatMarketo Engage屬性**：將未使用的Marketo Engage訂閱中的Dynamic Chat屬性取消同步，可幫助您促進資料清理，並視需要同步替代屬性。

## 新一代體驗

**新的切換切換器檢視**：以下檢視現在可用於新一代體驗：

* [電子郵件詳細資料檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [電子郵件清單檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 體驗自動化 {#experience-automation}

* **全域表單欄位驗證規則排除**：將特定表單從全域表單驗證規則中排除，以便訂閱中心和其他關鍵業務工作流程可以接受所有值。

* **自助服務流程步驟**：藉由撰寫自訂的流程步驟以用於Smart Campaigns的功能，擴展Marketo Engage與棧疊其餘部分之間的連線。 Marketo Engage使用者和合作夥伴均可運用此功能，在「觸發器」、「批次」和「可執行促銷活動」中使用外部Web服務，而非Webhook，後者只能用於「觸發促銷活動」。

* **Munchkin通訊協定不可知的連結追蹤**：擴充對追蹤的支援 `tel` 和 `mailto` 使用Munchkin追蹤擴充的網頁行為集的連結。

* **適用於Webhook的其他HTTP方法**：將PUT、PATCH和DELETE指定為與Web服務互動的請求型別。

## 銷售分析 {#sales-insight}

![（星號）](assets/yellow-star.png)

* **在Salesforce中設定銷售分析許可權**：管理員可以透過Marketo App許可權集（隸屬於Sales Insight Salesforce套件的一部分），提供使用者層級上有限一組人員的銷售分析存取權，而不是設定檔層級。

* **我的Marketo動態磚更新 — 銷售分析動作**：Marketo管理員（及其指派的使用者）現在可以透過位於「我的Marketo」頁面上的新「銷售分析動作」圖磚，快速導覽至其「銷售分析動作」執行個體。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **Salesforce API更新**：透過Salesforce 2022年夏季發行版本，Salesforce將不再支援API舊版21-30。 透過此Marketo Engage版本，所有使用舊版API的Sales Connect請求都已更新，以保持在支援的版本。 如需Salesforce API處分計畫的完整詳細資訊，請按一下 [此處](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## API增強功能 {#api-enhancements}

* **大量計畫成員擷取API的新篩選功能**：依方案會員資格狀態、updatedAt、cadence或用盡的內容來篩選，以調整擷取的資料集。

* **大量計畫成員擷取API改善**：在建立工作期間指定最多10個程式，以改善輸送量。

## 公告 {#announcements}

* **Forms淘汰 — Forms 1.0、銷售機會擷取/儲存端點，以及無指令碼版本的表單**：對Forms 1.0資產的支援將於2022年10月前從Marketo Engage中完全移除。 所有現有的Forms 1.0資產都將停止運作。 Marketo Engage表單需要在登陸頁面和網站上載入JavaScript。

**_產品發行網路研討會_**

[2022年6月和8月Marketo Engage版本網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
