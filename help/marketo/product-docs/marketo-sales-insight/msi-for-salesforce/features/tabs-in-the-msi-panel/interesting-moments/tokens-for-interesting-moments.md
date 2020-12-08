---
unique-page-id: 1146999
description: 精彩瞬間的代號——行銷檔案——產品檔案
title: 有趣時刻的Token
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 有趣時刻的Token {#tokens-for-interesting-moments}

>[!NOTE]
>
>**必要條件**
>
>* 瞭解如何使用「 [有趣的時刻」流程步驟](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)。
>* 進一步瞭解 [Token](http://docs.marketo.com/display/docs/tokens)。

>



## 可用預付碼 {#available-tokens}

查看 [Token概觀](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) ，查看您可放入有趣時刻的所有Token。

## 觸發Token {#trigger-tokens}

根據智慧型促銷活動中使用的觸發器，會提供額外的觸發器Token。

* `{{trigger.Trigger Name}}` 這總是觸發器本身。 例如：按一下電子郵件中的連結。
* `{{trigger.Name}}` 是觸發促銷活動的資產名稱。 例如：網頁上的「點按連結」是URL本身、Salesforce觸發程式的主題等。
* 其他觸發程式會根據限制提供，如下所示：

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
  </tr> 
  <tr> 
   <td>取消訂閱電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
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
   <td><br></td> 
  </tr> 
  <tr> 
   <td>已傳送銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>開啟銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>收到的銷售電子郵件</td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾號）"></td> 
  </tr> 
  <tr> 
   <td colspan="1">銷售電子郵件已反彈</td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾號）"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾號）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
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
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">瀏覽網頁*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾號）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾號）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果它沒有勾選（勾選） ![](assets/check.svg) ，則會在有趣的時刻傳回空字串（無）。

*「觸發瀏 **覽」網頁** ，有幾個額外的Token:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>請隨時測試您的有趣時刻，以確保呈現您想要的方式。
>
>此外，請務必讓銷售人員感興趣，而不只是您。 ![（眨眼）](assets/wink.svg)>

