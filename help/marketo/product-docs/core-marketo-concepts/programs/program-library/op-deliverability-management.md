---
description: OP — 傳遞能力管理 — Marketo檔案 — 產品檔案
title: OP — 傳遞性管理
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 4%

---

# OP — 傳遞性管理 {#op-deliverability-management}

這是傳遞能力管理最佳實務工作流程的範例，利用Marketo Engage預設程式來檢視您目前的電子郵件傳遞能力狀態，並管理長期跳出和未回應者。

>[!NOTE]
>
>需要自訂字串欄位「行銷暫停原因」才能匯入。 [深入瞭解](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}。

如需進一步的策略協助或自訂方案的協助，請連絡Adobe客戶團隊或造訪[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}頁面。

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

## 先決條件欄位 {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>類型</th> 
   <th>易記名稱</th>
   <th>API名稱</th>
  </tr>
  <tr> 
   <td>字串</td> 
   <td>行銷活動暫停原因</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Smart Campaign</td> 
   <td> </td>
   <td>行銷暫停長期無回應者</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>行銷暫停長期退回的電子郵件</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>在電子郵件更新後重設「電子郵件無效」</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>電子郵件更新後重設「行銷活動已暫停」</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>管理</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>檢閱</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

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

## 最佳實務 {#best-practices}

* 每個建立的行銷活動旨在作為最佳實務建立的範例，而不是特定於您的使用案例。 請記得更新Smart Campaign，以解決您的特定痛點和資料挑戰。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。
