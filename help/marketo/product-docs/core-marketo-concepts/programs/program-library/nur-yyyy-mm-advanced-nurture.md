---
description: NUR-YYYY-MM-Advanced Nurture - Marketo檔案 — 產品檔案
title: NUR-YYYY-MM-Advanced Nurture
feature: Programs
exl-id: cd266cad-843b-4329-ad40-2f3d0acd4948
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 3%

---

# NUR-YYYY-MM-Advanced Nurture {#nur-yyyy-mm-advanced-nurture}

這是使用Marketo Engage參與計畫的進階Nurture計畫範例。 巢狀電子郵件程式會防止使用者接收他們已使用的內容，或控制他們應在每個資料流中使用的內容型別。 歸因報表可針對每個個別巢狀電子郵件程式執行。 管道： 「Nurture」以及巢狀電子郵件計畫的專用「Nurture電子郵件」管道會利用Marketo Engage電子郵件計畫傳送一封電子報電子郵件。 電子郵件可以包含或不包含A/B測試。

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
   <td>培養</td> 
   <td>01 — 成員 
<br/>02 — 參與 — 成功</td>
   <td>包含</td>
   <td>參與</td>
  </tr>
  <tr> 
   <td>Nurture電子郵件</td> 
   <td>01 — 略過 
<br/>02 — 已傳送
<br/>03 — 參與 — 成功</td>
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
   <td>巢狀方案</td> 
   <td> </td>
   <td>01 — 主題X</td>
  </tr>
  <tr> 
   <td>巢狀方案</td> 
   <td> </td>
   <td>02 — 主題Y</td>
  </tr>
  <tr> 
   <td>巢狀方案</td> 
   <td> </td>
   <td>03 — 主題Z</td>
  </tr>
  <tr> 
   <td>電子郵件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>01 — 電子郵件（在巢狀程式中上線）</td>
  </tr>
   <tr> 
   <td>電子郵件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>02 — 電子郵件（在巢狀程式中上線）</td>
  </tr>
   <tr> 
   <td>電子郵件</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">快速入門電子郵件範本</a></td>
   <td>03 — 電子郵件（在巢狀程式中上線）</td>
  </tr>
  <tr> 
   <td>本地報告</td> 
   <td> </td>
   <td>電子郵件效能</td>
  </tr>
  <tr> 
   <td>本地報告</td> 
   <td> </td>
   <td>電子郵件連結效能</td>
  </tr>
  <tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 — 加入Nurture</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 — 暫停Nurture</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>03 — 繼續培養</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>04 — 參與（計畫成功）</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>00 — 略過電子郵件（位於每個巢狀方案中）</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 — 傳送電子郵件（位於每個巢狀方案）</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 — 參與成功（位於每個巢狀方案中）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>資產（包含巢狀程式和資產資料夾也位於巢狀程式中以包含電子郵件）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>巢狀程式（位於「資產」資料夾下）</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>行銷活動 — 在上層Nurture方案中容納所有智慧行銷活動，行銷活動資料夾也位於每個巢狀方案中</td>
  </tr>
  <tr> 
   <td>資料夾</td> 
   <td> </td>
   <td>報表</td>
  </tr>
 </tbody> 
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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

* 請考慮更新您匯入的程式中的範本，以使用目前品牌的範本，或更新新匯入的範本，以透過新增程式碼片段或適當的標誌/頁尾資訊來反映您的品牌。

* 請考慮更新此程式範例的命名慣例，以符合您的命名慣例。

* 確定您已有規則可暫停並繼續您的Nurture步調。 這些智慧行銷活動應在參與方案啟動之前啟動或排程。

>[!NOTE]
>
>請記得在程式範本上更新「我的Token值」，並且每次您視需要使用程式時都進行更新。

>[!TIP]
>
>別忘了啟動「04 — 參與（方案成功）」行銷活動以追蹤成功！ 執行此動作 _早於_ 您的電子郵件已傳送。
