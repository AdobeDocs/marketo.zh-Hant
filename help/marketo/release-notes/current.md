---
description: 當前發行說明 — Marketo文檔 — 產品文檔
title: 當前發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 375af5ec7293acd0cdf352c8aa0a7a3973b248be
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# 發行說明：2022年6月 {#release-notes-june-22}

在下面，您將找到6月22日發行版中包含的所有功能。 查看您的Adobe Marketo Engage版功能的可用性。

>[!AVAILABILITY]
>
>用星表示的特徵(![星](assets/yellow-star.png))是付費附加項。 請聯繫您的Marketo Engage代表以瞭解詳細資訊。

以下功能將開始在 **2022年6月24日**，在隨後的幾週內分階段部署剩餘功能（除非另有說明）。

## 營銷資料環境 {#marketing-data-environment}

* **公開自定義對象的CreatedAt/UpdatedAt欄位**:使您能夠在「人員詳細資訊」螢幕中檢查這些欄位，以獲得更多的洞察力。

## 跨通道業務流程 {#cross-channel-orchestration}

* **改進的流設計器動態聊天可用性**:直接從流設計器畫布添加卡，無需拖放。 動態聊天介面也已改進，以提供對單個卡中內容的更好的可視性。

* **動態聊天的高級約會路由規則**:動態聊天為目標約會路由提供了更多選項。 根據Marketo Engage屬性指定應路由哪些代理約會，確保將銷售線索路由到相應的代理。

* **動態聊天的高級對話框報告**:使用針對項目和轉換指標的全新資料可視化功能，更詳細地查看動態聊天活動的績效。

* **動態聊天的未使用Marketo Engage屬性未同步**:取消同步動態聊天訂閱中未使用的Marketo Engage屬性，幫助您簡化資料清潔，並允許根據需要同步其他屬性。

## 體驗自動化 {#experience-automation}

* **全局表單域驗證規則排除**:從全局表單驗證規則中排除特定表單，以便訂閱中心和其他關鍵業務工作流可以接受所有值。

* **自助流步驟**:通過編寫自定義流步驟以便在智慧市場活動中使用，擴展Marketo Engage與堆棧其餘部分之間的連接。 Marketo Engage用戶和合作夥伴都可以利用此功能，允許在「觸發」、「批處理」和「可執行」市場活動中使用外部Web服務，而Webhooks只能在「觸發」市場活動中使用。

* **Munchkin協定不可知鏈路跟蹤**:擴展對跟蹤的支援 `tel` 和 `mailto` 與Munchkin連結以跟蹤擴展的Web行為集。

* **用於Webhooks的其他HTTP方法**:將PUT、PATCH和DELETE指定為與Web服務交互的請求類型。

## 銷售洞察 {#sales-insight}

![（星號）](assets/yellow-star.png)

* **Salesforce中的Sales Insight權限集**:管理員可以通過Sales Insight Salesforce包的一部分Marketo應用權限集，為用戶級別上的有限人員集提供Sales Insight訪問權限，而不是配置檔案級別。

## API增強 {#api-enhancements}

* **批量程式成員提取API的新篩選功能**:按程式成員身份狀態、updatedAt、cadence或已用盡的內容篩選以細化提取的資料集。

* **批量程式成員提取API改進**:在建立作業期間指定最多10個程式以提高吞吐量。

## 公告 {#announcements}

* **Forms棄用 — Forms1.0、引導捕獲/保存終結點和表單的無指令碼版本**:對Forms1.0資產的支援將完全從Marketo Engage中取消。 所有Forms1.0現有資產將停止運作。 Marketo Engage表單需要JavaScript載入到登錄頁和網站上。

**_產品發佈網路研討會_**

在2022年8月24日上午9:00 AM PT / 12:00 PM ET, [即時網路研討會](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html)由我們的產品團隊托管的{target=&quot;_blank&quot;}，您可以在其中學習如何使用所有最新的產品創新。
