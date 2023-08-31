---
description: OP — 資料管理 — Marketo檔案 — 產品檔案
title: 作業資料管理
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 5aa0c2e3be16219613f0c72235428a962f8d58b3
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 2%

---

# 作業資料管理 {#op-data-management}

這是使用預設程式的簡單作業資料管理最佳實務工作流程的範例，協助您管理Marketo Engage資料庫中記錄的資料一致性。

如需進一步的策略協助或自訂方案，請聯絡Adobe客戶團隊或造訪 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} 頁面。

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

## 程式包含下列資產 {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>類型</th> 
   <th>範本名稱</th>
   <th>資產名稱</th>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>標準化國家/地區 — 美國</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>標準化國家 — 英國</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>將封鎖清單設為True</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>將Is Partner設為True</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>清單匯入</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>直播活動</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>線上廣告</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>貿易展</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>網頁內容</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>網路請求</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>網路研討會</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>從清單匯入新增人員</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>從直播活動中新增人員</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>從線上廣告新增人員</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>貿易展的新人員</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>從網路內容新增人員</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>從網路請求新增人員</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>網路研討會的新人員</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>人員來源夜間批次（適用於高流量例項）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>已觸發個人來源（針對低流量例項）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>擷取個人來源</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>標準化</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>記錄管理</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>封鎖清單</td>
  </tr>
 </tbody> 
</table>

程式熒幕擷圖

## 衝突規則 {#conflict-rules}

* **計畫標籤**
   * 在此訂閱中建立標籤 —  _建議_
   * 忽略

* **具相同名稱的登陸頁面範本**
   * 複製原始範本 —  _建議_
   * 使用目的地範本

* **具有相同名稱的影像**
   * 保留兩個檔案 —  _建議_
   * 取代此訂閱中的專案

* **相同名稱的電子郵件範本**
   * 保留兩個範本 —  _建議_
   * 取代現有範本

衝突規則的熒幕擷圖

## 最佳實務 {#best-practices}

* 每個建立的行銷活動旨在作為最佳實務建立的範例，而不是特定於您的使用案例。 請記得更新Smart Campaign，以解決您的特定痛點和資料挑戰。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。
