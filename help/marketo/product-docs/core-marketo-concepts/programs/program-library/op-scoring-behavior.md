---
description: OP-Scoring-Behavior - Marketo檔案 — 產品檔案
title: OP-評分-行為
feature: Programs
exl-id: c564a301-0054-431a-8f0f-0299cd91b59c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 22%

---

# OP-評分-行為 {#op-scoring-behavior}

此範例是使用Marketo Engage預設程式的行為評分進階（代碼化）作業程式。 在方案的「我的Token」索引標籤下檢視和編輯評分值。 需要名為「行為分數」的自訂分數欄位。

如需進一步的策略協助或自訂方案的協助，請連絡Adobe客戶團隊或造訪[Adobe Professional Services](https://business.adobe.com/tw/customers/consulting-services/main.html){target="_blank"}頁面。

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
   <td>分數</td>
   <td>行為分數</td>
   <td>行為分數</td>
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
   <td>電子郵件 — 按一下電子郵件中的連結</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>表單 — 填寫聯絡人表單</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>表單 — 填寫內容表單</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>表單 — 填寫預設表單</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>表單 — 填寫事件表單</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>網頁 — 下載任何PDF</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>網頁 — PPC評分</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>網頁 — 造訪重要網頁</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>網頁 — 在1天內造訪多個網頁</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>即時活動 — 已出席</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>商展 — 受影響</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>商展 — 造訪的展位</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>網路研討會 — 已參加</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>降低分數 — 無活動</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>降低分數 — 造訪不想要的網頁</td>
  </tr>
  <tr>
   <td>資料夾</td>
   <td> </td>
   <td>互動</td>
  </tr>
  <tr>
   <td>資料夾</td>
   <td> </td>
   <td>計畫狀態變更</td>
  </tr>
  <tr>
   <td>資料夾</td>
   <td> </td>
   <td>分數耗損</td>
  </tr>
 </tbody>
</table>

![](assets/op-scoring-behavior-1.png)

## 包含我的Token {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>權杖型別</th>
   <th>代號名稱</th>
   <th>價值</th>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Decrease Score - No Activity}}</code></td>
   <td>-10</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Decrease Score - Visits Undesirable Web Pages}}</code></td>
   <td>-5</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Email - Clicks Link}}</code></td>
   <td>+2</td>
  </tr>
   <tr>
   <td>分數</td>
   <td><code>{{my.Form - Fills Out Contact Form}}</code></td>
   <td>+30</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Form - Fills Out Content Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Form - Fills Out Default Form}}</code></td>
   <td>+10</td>
  </tr>
   <tr>
   <td>分數</td>
   <td><code>{{my.Form - Fills-out Event Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Live Event - Attended}}</code></td>
   <td>+30</td>
  </tr>
   <tr>
   <td>分數</td>
   <td><code>{{my.Tradeshow - Influenced}}</code></td>
   <td>+20</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Tradeshow - Visited Booth}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Web - Downloaded Any PDF}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Web - PPC Scoring}}</code></td>
   <td>+15</td>
  </tr>
   <tr>
   <td>分數</td>
   <td><code>{{my.Web - Visits Key Web Pages}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Web - Visits Multiple Web Pages in 1 Day}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>分數</td>
   <td><code>{{my.Webinar - Attended}}</code></td>
   <td>+20</td>
  </tr>
 </tbody>
</table>

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

* 每個建立的行銷活動都是最佳實務建立的範例，而非使用案例所特有的。 請記得更新Smart Campaign，以解決您的特定痛點和資料挑戰。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。
