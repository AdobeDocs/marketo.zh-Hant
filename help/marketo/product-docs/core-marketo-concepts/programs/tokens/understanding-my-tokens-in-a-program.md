---
unique-page-id: 1147114
description: 了解方案中的代號 — Marketo檔案 — 產品檔案
title: 了解程式中的代號
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# 了解程式中的代號 {#understanding-my-tokens-in-a-program}

代號是變數，您可在電子郵件、登錄頁面和智慧型行銷活動中使用，讓您的生活更輕鬆。

除了「我的代號」，您也可以在程式中使用任何內建的代號。 查看 [Token概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## 我的代號  {#my-tokens}

我的代號是任何人都能建立的自訂變數。 是 [已建立](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 在campaign資料夾或方案中。

我的代號顯示如下： `{{my.Name Of Token}}`

範例:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>代號類型</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>日曆檔案 <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此代號來 <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">新增日曆事件檔案(.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> 至您的電子郵件和登錄頁面。</td> 
  </tr> 
  <tr> 
   <td><p>日期 <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>此代號包含日期值。 日期會顯示為年月日(例如2016-05-23)。</td> 
  </tr> 
  <tr> 
   <td>電子郵件指令碼 <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此代號在您的電子郵件中執行Velocity指令碼。 深入了解 <a href="https://developers.marketo.com/documentation/email-scripting/" title="追蹤連結" rel="nofollow">此處</a>. </td> 
  </tr> 
  <tr> 
   <td>數字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任何整數。 甚至可能是負面的。</td> 
  </tr> 
  <tr> 
   <td>RTF <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>這是HTML。 在電子郵件和登錄頁面中使用。</td> 
  </tr> 
  <tr> 
   <td>分數 <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>在 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">變更分數流程步驟</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC促銷活動 <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">使用此代號可允許成為Marketo計劃一部分的銷售機會也添加到添加的任何SFDC促銷活動中。</td> 
  </tr> 
  <tr> 
   <td>文字 <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>只發些簡訊。 當HTML超量時使用。 文字代號的大小限制為524,288個字元(UTF-8)或2 MB。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>在Microsoft Dynamics或Salesforce上從Sales Insight傳送電子郵件時，無法解析我的代號；只會填入標準代號（銷售機會、公司等）。 代號的預設值 _will_ 不過，還是有用。

## 巢狀代號 {#nesting-tokens}

建立新令牌時，樹中的其他對象可以引用該令牌。 此為建立代號的命名結構，以方便管理。

* **本機代號：** 代號是在該程式或資料夾中建立的。
* **繼承的Token:** 代號是在樹狀結構中某處建立的，位於較高層的程式或資料夾中。
* **被覆蓋的令牌：** 代號已繼承，然後有人在此程式或資料夾中做了例外。

您可以建立全域變數，然後在樹狀結構中的較低層級覆寫它們。

移動程式和資料夾也會影響代號。 請務必確認在移動期間參照未損毀。

>[!NOTE]
>
>如果您從參與方案傳送的電子郵件是預設方案的子電子郵件（不是您參與方案的本機電子郵件），則電子郵件中使用的任何「我的代號」都會從子電子郵件所在的預設方案中解析。

>[!MORELIKETHIS]
>
>* [Token概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [管理我的代號](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

