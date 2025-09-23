---
description: CT-YYYY-MM-Content非Marketo登陸頁面 — Marketo檔案 — 產品檔案
title: CT-YYYY-MM-非 Marketo 登陸頁面上的內容
feature: Programs
exl-id: b7cf8e52-4f3f-44d7-ab4c-ad10fa0badc9
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 9%

---

# CT-YYYY-MM-非 Marketo 登陸頁面上的內容 {#ct-yyyy-mm-content-non-marketo-landing-page}

此範例為含有Marketo Engage表單的內容程式範例，此程式可利用Marketo Engage預設程式在非Marketo Engage登陸頁面上下載內容。 此程式旨在搭配您網站上內嵌的Marketo Engage表單使用。 優惠/內容的連結可在感謝電子郵件中傳送。

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
   <td>網頁內容</td>
   <td>01位成員
<br/>02 — 參與 — 成功</td>
   <td>包含</td>
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
   <td>電子郵件</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速開始電子郵件範本</a></td>
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
   <td>智慧行銷活動</td>
   <td> </td>
   <td>00 — 擷取贏取計畫</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>01填寫表單</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>02參與（計畫成功）</td>
  </tr>
  <tr>
   <td>資料夾</td>
   <td> </td>
   <td>Assets — 容納所有創意資產
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
   <td>報告</td>
  </tr>
 </tbody>
</table>

![](assets/ct-yyyy-mm-content-non-marketo-landing-page-1.png)

## 包含我的Token {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>權杖型別</th>
   <th>代號名稱</th>
   <th>價值</th>
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

* **程式標籤**
   * 在此訂閱中建立標籤 — _建議_
   * 忽略

* **名稱相同的登入頁面範本**
   * 複製原始範本
   * 使用目的地範本 — _建議_

* **相同名稱的影像**
   * 保留兩個檔案
   * 取代此訂閱中的專案 — _建議_

* **相同名稱的電子郵件範本**
   * 保留兩個範本
   * 取代現有的範本 — _建議_

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
>別忘了啟動「02參與」行銷活動以追蹤成功！ _before_&#x200B;請執行此動作。您的表單已上線且已傳送電子郵件。
