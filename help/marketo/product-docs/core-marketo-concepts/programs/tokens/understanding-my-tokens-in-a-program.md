---
unique-page-id: 1147114
description: 瞭解我的代號在計畫-Marketo文檔——產品文檔
title: 瞭解程式中的Token
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 瞭解程式中的My Token {#understanding-my-tokens-in-a-program}

Token是一個變數，您可在電子郵件、登陸頁面和智慧型促銷活動中使用，讓您的生活更輕鬆。

除了「我的Token」（代號）外，您也可以在程式中使用任何內建Token。 請參閱[Token概觀](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)。

## 我的代號{#my-tokens}

我的Token是任何人都能建立的自訂變數。 它們在促銷活動資料夾或程式中都是[created](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)。

我的Token會顯示如下：`{{my.Name Of Token}}`

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
   <td>日曆檔案 <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此Token將日曆事件檔案(.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a>新增至您的電子郵件和登陸頁面。<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md"></a></td> 
  </tr> 
  <tr> 
   <td><p>日期 <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>此代號包含日期值。 日期會顯示為年月日（例如2016-05-23）。</td> 
  </tr> 
  <tr> 
   <td>電子郵件指令碼 <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此Token，在電子郵件中執行Velocity指令碼。 進一步瞭解<a href="https://developers.marketo.com/documentation/email-scripting/" title="追蹤連結" rel="nofollow">此處</a>。 </td> 
  </tr> 
  <tr> 
   <td>編號<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任何整數。 甚至可能是負面的。</td> 
  </tr> 
  <tr> 
   <td>Rich Text <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>這是HTML。 在電子郵件和登陸頁面中使用。</td> 
  </tr> 
  <tr> 
   <td>分數 <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>在<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">變更分數流程步驟</a>中使用此Token。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC促銷活動 <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">使用此代號可讓成為Marketo計劃一部分的銷售機會也添加到添加的任何SFDC促銷活動中。</td> 
  </tr> 
  <tr> 
   <td>文字 <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>只要一些文字。 當HTML過度檢視時使用。 文字Token的大小限制為524,288個字元(UTF-8)或2 MB。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>在Microsoft Dynamics或Salesforce上，從Sales Insight傳送電子郵件時，My Token無法解析；只會填入標準Token（銷售機會、公司等）。 不過，Token _的預設值將_&#x200B;運作。

## 巢狀代號{#nesting-tokens}

當您建立新的Token時，樹狀結構中的其他物件可參照它。 Token的建立位置有命名結構，以方便管理。

* **本機Token:** 此Token就建立在該程式或資料夾中。
* **繼承的Token:** Token是在較高層級程式或資料夾的樹狀結構中建立。
* **覆寫的Token:** Token已繼承，然後有人在此程式或資料夾中發生例外。

您可以建立全域變數，然後在樹狀結構的較低層級覆寫這些變數。

移動程式和資料夾也會影響Token。 請務必檢查，以確定在移動期間參照未損壞。

>[!NOTE]
>
>如果您從參與計畫傳送的電子郵件是預設計畫的子電子郵件（非您的參與計畫的本機），則電子郵件中使用的任何My Token都會從子電子郵件所在的預設計畫中解決。

>[!MORELIKETHIS]
>
>* [預付碼概觀](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [管理我的代號](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

