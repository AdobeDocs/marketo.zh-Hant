---
description: TS-YYYY-MM-DD-Tradeshow計畫 — Marketo檔案 — 產品檔案
title: TS-YYYY-MM-DD-Tradeshow計畫
feature: Programs
exl-id: 39ef8d6e-392b-456e-a925-b1f6c2cb81d8
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 7%

---

# TS-YYYY-MM-DD-Tradeshow計畫 {#ts-yyyy-mm-dd-tradeshow-program}

這是商展計畫的範例，包含利用Marketo Engage活動計畫的邀請和後續電子郵件。

如需進一步的策略協助或自訂方案的協助，請連絡Adobe客戶團隊或造訪[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}頁面。

## 頻道摘要 {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>頻道</th>
   <th>成員資格狀態</th>
   <th>Analytics行為</th>
   <th>計畫型別</th>
  </tr>
  <tr>
   <td>活動</td>
   <td>01 — 已邀請
   <br/>02已輪候
   <br/>03已註冊
   <br/>04個造訪的攤位
   <br/>05參與在展示 — 成功
   <br/>06參與發佈會 — 成功</td>
   <td>包含</td>
   <td>活動</td>
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
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>01 — 電子郵件 — 感謝您</td>
  </tr>
   <tr>
   <td>電子郵件</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>02a — 電子郵件 — 邀請</td>
  </tr>
  <tr>
  <tr>
   <td>本地報告</td>
   <td> </td>
   <td>電子郵件效能</td>
  </tr>
  <tr>
   <td>本地報告</td>
   <td> </td>
   <td>計畫績效</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>00 — 擷取贏取計畫</td>
  </tr>
  <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>01 — 傳送邀請</td>
  </tr>
   <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>02 — 傳送後續追蹤電子郵件</td>
  </tr>
   <tr>
   <td>智慧行銷活動</td>
   <td> </td>
   <td>03 — 透過後續追蹤電子郵件參與（成功）</td>
  </tr>
  <tr>
   <td>資料夾</td>
   <td> </td>
   <td>Assets — 容納所有創意資產
<br/>（電子郵件和登陸頁面的子資料夾）</td>
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

![](assets/ts-yyyy-mm-dd-tradeshow-program-1.png)

## 包含我的Token {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>權杖型別</th>
   <th>代號名稱</th>
   <th>值</th>
  </tr>
  <tr>
   <td>行事曆檔案</td>
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>按兩下以取得詳細資料</td>
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
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
   <tr>
   <td>RTF文字</td>
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr>
   <td>文字</td>
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr>
   <td>文字</td>
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
  <tr>
   <td>文字</td>
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr>
   <td>文字</td>
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr>
   <td>文字</td>
   <td><code>{{my.Event-Type}}</code></td>
   <td>商展</td>
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

* 匯入網路研討會計畫後，將表單從本機資產移至位於Design Studio中的全域資產。
   * 減少Design Studio的表單數量並運用更多全域資產，可讓您的程式設計和管理管理擁有更多擴充性。 此外，欄位、選擇加入語言等的定期合規性更新也有彈性。

* 請考慮更新您匯入的程式中的範本，以使用目前品牌的範本，或更新新匯入的範本，以透過新增程式碼片段或適當的標誌/頁尾資訊來反映您的品牌。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。

>[!NOTE]
>
>請記得在程式範本上更新「我的Token值」，並且每次您視需要使用程式時都進行更新。

>[!TIP]
>
>別忘了啟用「03 — 透過追蹤電子郵件參與（方案成功）」行銷活動以追蹤成功！ 請在&#x200B;_之前執行此動作，您的電子郵件已寄出。_

>[!IMPORTANT]
>
>參考URL的Token不可包含http://或https:// ，否則連結在資產中無法正常運作。
