---
description: Marketo LP內容 — Marketo檔案 — 產品檔案
title: Marketo LP上的內容
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# Marketo LP上的內容 {#content-on-marketo-lp}

程式名稱： Marketo LP上的CT-YYYY-MM-Content

此範例參考資料設計作為內容程式，可利用Marketo登陸頁面和Marketo表單，並運用Marketo預設程式。 此表單用於存取內容/選件。 優惠連結可顯示在感謝頁面上、以感謝電子郵件傳送或兩者皆顯示。 如需進一步的策略協助或自訂方案，請聯絡Adobe客戶團隊或造訪 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) 頁面。

**頻道摘要**

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

**程式包含以下資產：**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>類型</th> 
   <th>範本名稱</th>
   <th>資產名稱</th>
  </tr> 
  <tr> 
   <td>電子郵件</td> 
   <td>快速入門電子郵件範本</td>
   <td>01 — 電子郵件 — 感謝您</td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td>快速入門LP範本</td>
   <td>01 - LP — 註冊</td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td>快速入門LP範本</td>
   <td>02 - LP — 感謝您</td>
  </tr>
  <tr> 
   <td>表單</td> 
   <td> </td>
   <td>內容登錄檔單</td>
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
   <td>行銷活動 — 容納所有智慧行銷活動</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>報表</td>
  </tr>
 </tbody> 
</table>

熒幕擷圖 — 程式圖片

**包含我的Token：**

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
<br/>在「我的Token」標籤下方的方案層級編輯此內容說明。 
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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>文字</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL？不含http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>請參閱預設衝突規則的程式匯入指示。

**建議的匯入預設衝突規則：**

* 計畫標籤
   * 在此訂閱中建立標籤（預設） — 建議
   * 忽略

* 具相同名稱的登陸頁面範本
   * 複製原始範本（預設）
   * 使用目的地範本 — 建議

* 具有相同名稱的影像
   * 保留兩個檔案（預設）
   * 取代此訂閱中的專案 — 建議

* 相同名稱的電子郵件範本
   * 保留兩個範本（預設）
   * 取代現有範本 — 建議

熒幕擷圖 — 預設衝突規則的圖片

**建議的最佳作法：**

* Marketo Consulting最佳實務建議在匯入內容程式後，將表單從本機資產移至Marketo EngageDesign Studio中的全域資產。
   * 減少Design Studio的表單數量並運用更多全域資產，可讓您的程式設計和管理管理擁有更多擴充性。 此外，欄位、選擇加入語言等的定期合規性更新也有彈性。

* 請考慮更新您匯入的程式中的範本，以使用目前品牌的範本，或更新新匯入的範本，以透過新增代碼片段或適當的標誌和頁尾資訊來反映您的品牌。

* 如有需要，請考慮更新此方案範本的命名慣例，使其與您的命名慣例一致。

* 別忘了視需要更新程式範本上的「我的Token值」，而且每次您使用程式時都須更新。

* 如需進一步的策略協助或自訂方案，請聯絡您的Adobe客戶團隊或造訪 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) 頁面。

>[!TIP]
>
>別忘了啟動「02參與」行銷活動以追蹤成功！ 請在您的表單上線並傳送電子郵件之前執行此動作。

>[!NOTE]
>
>參考URL的Token不可包含http://或https:// ，否則連結在資產中無法正常運作。
