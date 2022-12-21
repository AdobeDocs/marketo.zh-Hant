---
unique-page-id: 1146999
description: 觸發Token以取得有趣的瞬間 — Marketo檔案 — 產品檔案
title: 觸發有趣時刻的代號
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
source-git-commit: f4c773ca76542827a498940f44b018ddb71816d6
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 觸發有趣時刻的代號 {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>了解如何使用 [有趣的力矩流步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## 可用Token {#available-tokens}

結帳 [Token概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) 來看看所有的代號。

## 觸發Token {#trigger-tokens}

根據智慧型行銷活動中使用的觸發器，可使用其他觸發器代號。

* `{{trigger.Trigger Name}}` 這總是實際觸發的本身。 例如：按一下電子郵件中的連結。
* `{{trigger.Name}}` 是觸發促銷活動的資產名稱。 例如：「網頁上的點按連結」是URL本身、Salesforce觸發器的主題等。
* 根據下列限制，提供其他觸發器。

**電子郵件觸發器**

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>點按電子郵件中的連結</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>硬電子郵件跳出數</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>電子郵件跳出數軟</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已傳送電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>開啟電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>已轉發給好友電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>已轉發給好友電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td>
  </tr> 
  <tr> 
   <td>從電子郵件取消訂閱</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Salesforce觸發器**

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>銷售電子郵件中的點按連結</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已發送銷售電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>開啟銷售電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>銷售電子郵件跳出數</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>收到銷售電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>已更新機會</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>所有者更改</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>人員已轉換</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>從SFDC中刪除人員</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>人員已同步至SFDC</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>從Opportunity中刪除</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>從SFDC促銷活動中移除</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>活動已記錄</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>活動已更新</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>添加到Opportunity</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>新增至SFDC Campaign</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>在SFDC促銷活動中狀態已變更</td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Sales Connect Triggers**

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>銷售電子郵件中的點按連結</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已發送銷售電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>開啟銷售電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>銷售電子郵件跳出數</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>收到銷售電子郵件</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已新增至Sales Campaign</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr>
   <td>所有者更改</td> 
   <td>已從Sales Campaign中移除</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已接收銷售呼叫</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**其他**

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>填寫表單</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>瀏覽網頁</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>點按網頁上的連結</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果沒有支票 ![（滴答）](assets/check.png) 然後，它會在有趣的時刻傳回空字串（無）。

&#42;觸發 **瀏覽網頁** 有一些額外的Token:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>總是測試一下你的有趣時刻，以確保它們以你想要的方式呈現。
>
>另外，確保對銷售人員來說有趣，而不只是對您！
