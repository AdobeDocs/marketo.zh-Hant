---
description: AWS移轉 — Marketo Engage檔案 — 產品檔案
title: AWS移轉
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 365a2c3767c8c3e3455361ac5c2a0e070796cbfa
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# AWS移轉 {#aws-migration}

在接下來的幾個月中，所有Marketo Engage訂閱都將從私人資料中心移轉至AWS公用雲端，以提升可靠性、擴充性和速度。

您將在移轉前約30天收到電子郵件和應用程式內通知。 使用本指南進行準備。

## 建議的動作

在移轉期間，所有Marketo Engage服務都將無法使用。 建議您採取下列步驟，以免對業務造成任何影響。

* **避免建立或更新銷售機會/人員**，或執行修改人員記錄的程式。

* **不要觸發後續程式**，因為排程的行銷活動將會暫停。

* **暫時停用所有傳送資料給Marketo Engage或從接收資料的整合**。

* **避免執行**&#x200B;資料匯入或匯出，或任何主要的銷售機會/人員產生行銷活動。

* **檢閱並更新IP允許清單**，以取得登入、API存取、電子郵件傳送、網頁追蹤和整合。

* **新增下列IP位址**，並將您目前的IP保持原樣：

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## 預期的服務影響

您無需對下列影響執行任何動作。

* **CRM整合和LaunchPoint服務**&#x200B;將會停用，但之後應該會自動繼續。
* **登陸頁面、表單和資料彙集**&#x200B;將無法使用，而將會顯示維護訊息。

## 排程 {#schedule}

新的日期和資料中心/Pod資訊會定期新增，因此請務必回到這裡檢視詳細資訊。

在檢閱下清單格之前，[請先瞭解如何識別](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)您的訂閱所在的資料中心和pod/伺服器。

<table>
 <tbody>
  <tr>
   <th style="width:50%">日期</th>
   <th style="width:20%">Pod</th>
   <th style="width:30%">時間</th>
  </tr>
  <tr>
   <td>2026年6月5日</td>
   <td>AB46</td>
   <td>下午5點（太平洋標準時間）</td>
  </tr>
  <tr>
   <td>2026年7月8日</td>
   <td>AB69<br>
   AB64</td>
   <td>下午5點（太平洋標準時間）<br>
   下午6點（太平洋標準時間）</td>
  </tr>
  <tr>
   <td>2026年7月9日</td>
   <td>AB70<br>
   AB43</td>
   <td>下午5點（太平洋標準時間）<br>
   下午6點（太平洋標準時間）</td>
  </tr>
  </body>
  </table>

## 更新與支援

如需最新更新，請將此頁面加入書籤。 如果您有任何問題，請透過Admin Console的支援入口網站或[Experience League](https://experienceleague.adobe.com/en/support)聯絡Adobe支援。
