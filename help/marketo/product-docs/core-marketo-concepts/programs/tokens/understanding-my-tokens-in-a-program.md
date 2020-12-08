---
unique-page-id: 1147114
description: 瞭解我的Token在計畫——行銷檔案——產品檔案
title: 瞭解程式中的Token
translation-type: tm+mt
source-git-commit: d78ecbec87d69cde66b583d21d7e0c95539bb6ec
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# 瞭解程式中的Token {#understanding-my-tokens-in-a-program}

Token是一個變數，您可在電子郵件、登陸頁面和智慧型促銷活動中使用，讓您的生活更輕鬆。

除了「我的Token」（代號）外，您也可以在程式中使用任何內建Token。 請參閱Token [概觀](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)。

## 我的預付碼  {#my-tokens}

我的Token是任何人都能建立的自訂變數。 它們是在 [促銷活動](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 資料夾或方案中建立的。

我的Token會顯示如下： `{{my.Name Of Token}}`

範例：

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
   <td>日曆檔案 <img alt="--" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此Token將日 <a href="../../../../product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">歷事件檔案(.</a><a href="../../../../product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">ics)新增至您的電子郵件和登陸頁面</a> 。</td> 
  </tr> 
  <tr> 
   <td><p>日期 <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>此代號包含日期值。 日期會顯示為年月日（例如2016-05-23）。</td> 
  </tr> 
  <tr> 
   <td>電子郵件指令碼 <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此Token，在電子郵件中執行Velocity指令碼。 在這裡進 <a href="http://developers.marketo.com/documentation/email-scripting/" title="追蹤連結" rel="nofollow">一步</a>。 </td> 
  </tr> 
  <tr> 
   <td>數字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任何整數。 甚至可能是負面的。</td> 
  </tr> 
  <tr> 
   <td>Rich Text <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>這是HTML。 在電子郵件和登陸頁面中使用。</td> 
  </tr> 
  <tr> 
   <td>分數 <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>在變更分數流程 <a href="../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">步驟中使用此Token</a>。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC促銷活動 <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">使用此代號可讓成為Marketo Program一部分的銷售機會也能新增至新增的任何SFDC促銷活動。</td> 
  </tr> 
  <tr> 
   <td>文字 <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>只要一些文字。 當HTML過度檢視時使用。 文字Token的大小限制為524,288個字元(UTF-8)或2 MB。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>在Microsoft Dynamics或Salesforce上，從Sales Insight傳送電子郵件時，My Token無法解析；只會填入標準Token（銷售機會、公司等）。 不過，代號的預 *設值* 仍能運作。

## 巢狀代號 {#nesting-tokens}

當您建立新的Token時，樹狀結構中的其他物件可參照它。 Token的建立位置有命名結構，以方便管理。

* **本機Token:** Token是直接在該程式或資料夾中建立。
* **繼承的Token:** 標籤是在樹狀結構中較高層級的程式或資料夾中建立的。
* **覆寫的Token:** 代號已繼承，然後有人在此程式或資料夾中做了例外。

您可以建立全域變數，然後在樹狀結構的較低層級覆寫這些變數。

移動程式和資料夾也會影響Token。 請務必檢查，以確定在移動期間參照未損壞。

>[!NOTE]
>
>如果您從參與計畫傳送的電子郵件是預設計畫的子電子郵件（非您的參與計畫的本機），則電子郵件中使用的任何My Token都會從子電子郵件所在的預設計畫中解決。

>[!MORELIKETHIS]
>
>* [預付碼概觀](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [管理我的代號](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

