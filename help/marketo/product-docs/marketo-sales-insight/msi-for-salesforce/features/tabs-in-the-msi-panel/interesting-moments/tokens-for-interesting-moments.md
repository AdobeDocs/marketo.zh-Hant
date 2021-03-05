---
unique-page-id: 1146999
description: 精彩瞬間的代號——行銷檔案——產品檔案
title: 有趣時刻的Token
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# 有趣時刻的代號{#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>瞭解如何使用[有趣的力矩流步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)。

## 可用預付碼{#available-tokens}

查看[Token Overview](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)，以查看您可放入有趣時刻的所有Token。

## 觸發Token {#trigger-tokens}

根據智慧型促銷活動中使用的觸發器，會提供額外的觸發器Token。

* `{{trigger.Trigger Name}}` 這總是觸發器本身。例如：按一下電子郵件中的連結。
* `{{trigger.Name}}` 是觸發促銷活動的資產名稱。例如：網頁上的「點按連結」是URL本身、Salesforce觸發程式的主題等。
* 其他觸發程式會根據約束提供，如下所示。

**電子郵件觸發程式**

<table> 
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
   <td>電子郵件中的點按連結</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>電子郵件彈回數硬</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>電子郵件彈回數軟體</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>電子郵件已傳送</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>已轉發給朋友的電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>轉寄給朋友的電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td>
  </tr> 
  <tr> 
   <td>取消訂閱電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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

<table> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已寄送銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>開啟銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>銷售電子郵件彈回數</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>業務機會已更新</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>擁有者變更</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>從SFDC刪除人員</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>人員與SFDC同步</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>新增至SFDC促銷活動</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>SFDC促銷活動中的狀態已更改</td> 
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

**Sales Connect觸發器**

<table> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已寄送銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>開啟銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>銷售電子郵件彈回數</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已新增至Sales Campaign</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>擁有者變更</td> 
   <td>已從Sales Campaign中移除</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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
   <td>收到銷售電話</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
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

<table> 
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
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>瀏覽網頁</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>在網頁上點按連結</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果它沒有勾選![(tick)](assets/check.svg)，則會在有意思的時刻傳回空字串（無）。

*觸發器&#x200B;**瀏覽網頁**&#x200B;包含一些額外的Token:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>請隨時測試您的有趣時刻，以確保呈現您想要的方式。
>
>此外，請務必讓銷售人員感興趣，而不只是您。 ![（眨眼）](assets/wink.svg)>
