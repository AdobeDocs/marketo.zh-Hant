---
description: 贏取API作業程式範本。 透過API用它來擷取潛在客戶。
title: OP-贏取-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
TQID: https://experienceleague.adobe.com/a-4w7mJg44cvotVtX2qwx1e4p8SKIbQU1jPWyQ0BzUA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: df401a2a-327d-468c-a5e4-b7b7ccd071a0id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 8%

---

# OP-贏取-API {#op-acquisition-api}

此範常式式適用於利用Marketo Engage預設程式來追蹤從API來源取得記錄的作業流程。

## 頻道摘要 {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>管道</th>
   <th>成員資格狀態</th>
   <th>Analytics行為</th>
   <th>計畫型別</th>
  </tr>
  <tr>
   <td>營運</td>
   <td>01位成員</td>
   <td>營運</td>
   <td>預設</td>
  </tr>
 </tbody>
</table>

## 程式包含下列Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>類型</th>
   <th>範本名稱</th>
   <th>資產名稱</th>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>設定贏取 — 批次</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>設定贏取 — 觸發器</td>
  </tr>
  <tr>
   <td>資料夾</td>
   <td> </td>
   <td>行銷活動（包含所有Smart Campaign）</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

## 衝突規則 {#conflict-rules}

* **程式標籤**
   * 在此訂閱中建立標籤 — _建議_
   * 忽略

* **名稱相同的登入頁面範本**
   * 複製原始範本 — _建議_
   * 使用目的地範本

* **相同名稱的影像**
   * 保留兩個檔案 — _建議_
   * 取代此訂閱中的專案

* **相同名稱的電子郵件範本**
   * 保留兩個範本 — _建議_
   * 取代現有範本

## 最佳做法 {#best-practices}

* 如果您需要在資料管理中趕上，請先執行批次促銷活動。

* 考慮使用類似的計畫，以確保與所有輸入來源的最佳做法一致，以包含您的CRM或資料整合。

* 在管道特定的管道行銷計畫中，確保必要時能擷取贏取。
