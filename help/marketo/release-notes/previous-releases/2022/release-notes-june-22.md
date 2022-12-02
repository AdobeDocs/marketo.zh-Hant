---
description: 發行說明 — 2022年6月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年6月
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
source-git-commit: 85e04fb8a52a417982014bc4bb101b6044e53f84
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 發行說明：2022年6月 {#release-notes-june-22}

以下是』22年6月版本包含的所有功能。 查看您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號表示的特徵(![星星](assets/yellow-star.png))是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

下列功能將於 **2022年6月24日**，並在後續數週分階段推出剩餘功能（除非另有指定）。

## 行銷資料環境 {#marketing-data-environment}

* **公開自訂物件的CreatedAt/UpdatedAt欄位**:讓您能夠在「人員詳細資訊」畫面中檢查這些欄位，以獲得更多深入分析。

## 跨管道協調 {#cross-channel-orchestration}

* **改善動態聊天的串流設計器可用性**:直接從串流設計工具畫布新增卡片，不需要拖放。 動態聊天介面也經過改良，可提供更清楚的個別資訊卡內容可見度。

* **動態聊天的高級約會路由規則**:動態聊天為目標約會傳送提供更多選項。 根據Marketo Engage屬性指定應路由哪些代理約會，以確保將銷售機會路由到相應的代理。

* **動態聊天的進階對話方塊報告**:使用參與和轉換量度的全新資料視覺效果，更詳細地檢視動態聊天促銷活動的效能。

* **取消同步動態聊天未使用的Marketo Engage屬性**:未使用的動態聊天訂閱會取消同步Marketo Engage屬性，協助您加速資料清潔度，並視需要同步替代屬性。

## 新一代體驗

**新切換開關視圖**:下列檢視現已可在新一代體驗中使用：

* [電子郵件詳細資訊檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target=&quot;_blank&quot;}
* [電子郵件清單檢視](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target=&quot;_blank&quot;}

## 體驗自動化 {#experience-automation}

* **全域表單欄位驗證規則排除**:從全域表單驗證規則中排除特定表單，讓訂閱中心和其他業務關鍵工作流程可以接受所有值。

* **自助流程步驟**:借由編寫可在智慧行銷活動中使用的自訂流程步驟，擴展Marketo Engage與堆疊其餘部分之間的連線。 Marketo Engage使用者和合作夥伴都可運用此功能，在觸發、批次和可執行促銷活動中使用外部Web服務，而Webhook僅能用於觸發促銷活動。

* **Munchkin協定無關連結追蹤**:延伸對追蹤的支援 `tel` 和 `mailto` 與Munchkin的連結，以追蹤擴充的網路行為集。

* **用於Webhook的其他HTTP方法**:將PUT、PATCH和DELETE指定為與網站服務互動的請求類型。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

* **Salesforce中設定的Sales Insight權限**:管理員可以透過Marketo應用程式權限集（Sales Insight Salesforce套件的一部分），在使用者層級（而非設定檔層級）為有限的一組人員提供Sales Insight存取權。

* **我的Marketo磁貼更新 — 銷售分析操作**:Marketo管理員（及其指定的使用者）現在可以透過「我的Marketo」頁面上新的「銷售分析動作」方塊，快速導覽至其「銷售分析動作」例項。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **Salesforce API更新**:隨著Salesforce Summer 22版本推出，Salesforce將不再支援API舊版21 -30。 在此Marketo Engage版本中，使用舊版API的所有Sales Connect請求均已更新，以保持在支援的版本內。 如需Salesforce API報廢計畫的完整詳細資訊，請按一下 [此處](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}。

## API增強功能 {#api-enhancements}

* **Bulk Program Member Extract API的新篩選功能**:依方案成員資格狀態、updatedAt、順序或用盡的內容篩選，以精簡擷取的資料集。

* **大量計畫成員提取API改進**:在建立工作期間指定最多10個程式，以提高吞吐量。

## 公告 {#announcements}

* **Forms淘汰 — Forms 1.0、Lead Capture/save端點，以及無指令碼的表單版本**:Forms 1.0資產的支援將於2022年10月前完全從Marketo Engage中移除。 所有現有的Forms 1.0資產將停止運作。 Marketo Engage表單需要JavaScript才能在登錄頁面和網站上載入。

**_產品發行網路研討會_**

[2022年6月和8月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target=&quot;_blank&quot;}
