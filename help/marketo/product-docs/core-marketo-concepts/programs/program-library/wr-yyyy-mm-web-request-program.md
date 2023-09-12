---
description: WR-YYYY-MM-Web請求計畫 — Marketo檔案 — 產品檔案
title: WR-YYYY-MM-Web請求程式
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 3%

---

# WR-YYYY-MM-Web請求程式 {#wr-yyyy-mm-web-request-program}

這是一個範例計畫，非常適用於使用Marketo Engage預設計畫的聯絡人請求、報價請求、示範請求或試用請求表單。 可與Marketo登陸頁面搭配使用，或作為非Marketo登陸頁面上的內嵌表單。 在提交表單時會傳送通知電子郵件給指定的個人。

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
   <td>網路請求</td> 
   <td>01 — 參與 — 成功</td>
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
   <td>表單</td> 
   <td> </td>
   <td>FM-WebRequestForm</td>
  </tr>
  <tr> 
   <td>電子郵件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>Alert-Webrequest</td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入門LP範本</a></td>
   <td>01 - LP — 要求</td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入門LP範本</a></td>
   <td>02 - LP — 感謝您</td>
  </tr>
  <tr> 
   <td>本地報告</td> 
   <td> </td>
   <td>登陸頁面績效</td>
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
   <td>資產 — 容納所有創意資產 
<br/>（警報和登陸頁面的子資料夾）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>行銷活動 — 容納所有智慧行銷活動</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>報表</td>
  </tr>
 </tbody> 
</table>

![](assets/wr-yyyy-mm-web-request-program-1.png)

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
   <td><code>{{my.Request-Type}}</code></td>
   <td>聯絡我們</td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL？不含http://</td>
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

* 匯入網路研討會計畫後，將表單從本機資產移至位於Design Studio中的全域資產。
   * 減少Design Studio的表單數量並運用更多全域資產，可讓您的程式設計和管理管理擁有更多擴充性。 此外，欄位、選擇加入語言等的定期合規性更新也有彈性。

* 請考慮更新您匯入的程式中的範本，以使用目前品牌的範本，或更新新匯入的範本，以透過新增程式碼片段或適當的標誌/頁尾資訊來反映您的品牌。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。

>[!NOTE]
>
>請記得在程式範本上更新「我的Token值」，並且每次您視需要使用程式時都進行更新。

>[!IMPORTANT]
>
>參考URL的Token不可包含http://或https:// ，否則連結在資產中無法正常運作。
