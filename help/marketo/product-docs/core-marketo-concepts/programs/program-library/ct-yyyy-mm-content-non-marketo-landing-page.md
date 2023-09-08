---
description: CT-YYYY-MM-Content非Marketo登陸頁面 — Marketo檔案 — 產品檔案
title: CT-YYYY-MM-Content非Marketo登陸頁面
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 3%

---

# CT-YYYY-MM-Content非Marketo登陸頁面 {#ct-yyyy-mm-content-non-marketo-landing-page}

此為具有Marketo Engage表單的內容程式範例，用於利用Marketo Engage預設程式在非Marketo Engage登陸頁面上下載內容。 此程式適用於使用內嵌在您的網站上的Marketo Engage表單。 優惠/內容的連結可在感謝電子郵件中傳送。

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
   <td>網頁內容</td> 
   <td>01位成員 
<br/>02參與成功</td>
   <td>包含</td>
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
   <td>電子郵件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>01 — 電子郵件 — 感謝您</td>
  </tr>
  <tr> 
   <td>表單</td> 
   <td> </td>
   <td>FM內容登錄檔單（Design Studio中的全域資產）</td>
  </tr>
  <tr> 
   <td>本地報告</td> 
   <td> </td>
   <td>電子郵件效能</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>00 — 擷取贏取計畫</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01填寫表單</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02參與（計畫成功）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>資產 — 容納所有創意資產 
<br/>（電子郵件和登陸頁面的子資料夾）  </td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>行銷活動 — 包含所有Smart Campaigns</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>報表</td>
  </tr>
 </tbody> 
</table>

![](assets/ct-yyyy-mm-content-non-marketo-landing-page-1.png)

## 包含我的Token {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>權杖型別</th> 
   <th>Token名稱</th>
   <th>值</th>
  </tr> 
  <tr> 
   <td>文字</td> 
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
 </tbody> 
</table>

## 衝突規則 {#conflict-rules}

* **計畫標籤**
   * 在此訂閱中建立標籤 —  _建議_
   * 忽略

* **具相同名稱的登陸頁面範本**
   * 複製原始範本
   * 使用目的地範本 —  _建議_

* **具有相同名稱的影像**
   * 保留兩個檔案
   * 取代此訂閱中的專案 —  _建議_

* **相同名稱的電子郵件範本**
   * 保留兩個範本
   * 取代現有範本 —  _建議_

## 最佳實務 {#best-practices}

* 匯入內容程式後，將表單從本機資產移至位於Design Studio中的全域資產。
   * 減少Design Studio的表單數量並運用更多全域資產，可讓您的程式設計和管理管理擁有更多擴充性。 此外，欄位、選擇加入語言等的定期合規性更新也有彈性。

* 請考慮更新您匯入的程式中的範本，以使用目前品牌的範本，或更新新匯入的範本，以透過新增程式碼片段或適當的標誌/頁尾資訊來反映您的品牌。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。

>[!NOTE]
>
>請記得在程式範本上更新「我的Token值」，並且每次您視需要使用程式時都進行更新。

>[!TIP]
>
>別忘了啟動「02參與」行銷活動以追蹤成功！ 執行此動作 _早於_ 您的表單已上線且已傳送電子郵件。
