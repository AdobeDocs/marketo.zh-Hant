---
description: OA-YYYY-MM-Online Advertising Marketo登陸頁面 — Marketo檔案 — 產品檔案
title: OA-YYYY-MM-Online Advertising Marketo登陸頁面
feature: Programs
exl-id: f7f17792-cc16-4a99-8683-68796770e42c
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 3%

---

# OA-YYYY-MM-Online Advertising Marketo登陸頁面 {#oa-yyyy-mm-online-advertising-marketo-landing-page}

此為線上廣告追蹤程式的範例，包含具有登錄檔單的Marketo登陸頁面，且使用Marketo預設程式。 優惠連結可顯示在感謝頁面上、以感謝電子郵件傳送或兩者皆顯示。

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
   <td>線上Advertising</td> 
   <td>01 — 成員 
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
   <td>表單</td> 
   <td> </td>
   <td>FM-Content註冊</td>
  </tr>
  <tr> 
   <td>電子郵件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>01 — 電子郵件 — 感謝您</td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入門LP範本</a></td>
   <td>01 - LP — 註冊</td>
  </tr>
   <tr> 
   <td>登陸頁面</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">快速入門LP範本</a></td>
   <td>02 - LP — 感謝您</td>
  </tr>
   <tr> 
   <td>本地報告</td> 
   <td> </td>
   <td>電子郵件效能</td>
  </tr>
  <tr> 
   <td>本地報告</td> 
   <td> </td>
   <td>登陸頁面績效</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>00 — 擷取贏取計畫</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 — 填寫表單</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 — 參與（計畫成功）</td>
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
   <td>報表</td>
  </tr>
 </tbody> 
</table>

![](assets/oa-yyyy-mm-online-advertising-marketo-landing-page-1.png)

## 包含我的Token {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>權杖型別</th> 
   <th>Token名稱</th>
   <th>值</th>
  </tr> 
  <tr> 
   <td>RTF文字</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>按兩下以取得詳細資訊  
<br/><code><--My Content Description Here--></code> 
<br/>在[我的Token]索引標籤下方的方案層級編輯此內容說明。 
<br/>您將能學習到： 
<li>專案符號1</li>
<li>專案符號2</li>
<li>專案符號3</li></td>
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
  <tr> 
   <td>文字</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL？不含http://</td>
  </tr>
 </tbody> 
</table>

程式熒幕擷圖

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

衝突規則的熒幕擷圖

## 最佳實務 {#best-practices}

* 匯入內容程式後，將表單從本機資產移至位於Design Studio中的全域資產。
   * 減少Design Studio的表單數量並運用更多全域資產，可讓您的程式設計和管理管理擁有更多擴充性。 此外，欄位、選擇加入語言等的定期合規性更新也有彈性。

* 請考慮更新您匯入的程式中的範本，以使用目前品牌的範本，或更新新匯入的範本，以透過新增程式碼片段或適當的標誌/頁尾資訊來反映您的品牌。

* 使用程式標籤，依您各種線上Advertising來源篩選報表。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。

>[!NOTE]
>
>請記得在程式範本上更新「我的Token值」，並且每次您視需要使用程式時都進行更新。

>[!TIP]
>
>別忘了啟動「02 — 參與（方案成功）」行銷活動以追蹤成功！ _before_&#x200B;請執行此動作。您的表單已上線且已傳送電子郵件。

>[!IMPORTANT]
>
>參考URL的Token不可包含http://或https:// ，否則連結在資產中無法正常運作。
