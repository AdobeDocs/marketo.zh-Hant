---
unique-page-id: 1147114
description: 瞭解程式中的我的Token - Marketo檔案 — 產品檔案
title: 了解方案中的我的權杖
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 4%

---

# 了解方案中的我的權杖 {#understanding-my-tokens-in-a-program}

代號是變數，可用於電子郵件、登陸頁面和智慧型行銷活動，讓您的生活更輕鬆。

除了「我的Token」，您也可以在程式中使用任何內建的Token。 檢視[Token概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}。

## 我的權杖  {#my-tokens}

我的Token是任何人都可以建立的自訂變數。 在本機上，它們是在[建立的行銷活動資料夾或方案中](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}。

我的Token顯示如下： `{{my.Name Of Token}}`

範例：

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table>
 <thead>
  <tr>
   <th>權杖型別</th>
   <th>說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>行事曆檔案 <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>使用此Token將<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">行事曆事件檔案(.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a>新增至您的電子郵件和登入頁面。</td>
  </tr>
  <tr>
   <td><p>日期 <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td>
   <td>此Token包含日期值。 日期會顯示為年 — 月 — 日（例如，2016-05-23）。</td>
  </tr>
  <tr>
   <td>電子郵件指令碼 <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>使用此代號在您的電子郵件中執行Velocity指令碼。 在<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/email-scripting" title="關注連結" rel="nofollow">此處</a>瞭解更多資訊。 </td>
  </tr>
  <tr>
   <td>數字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td>
   <td>任何整數。 甚至可以是負數。</td>
  </tr>
  <tr>
   <td>RTF文字 <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>這是HTML。 在電子郵件和登入頁面中使用。</td>
  </tr>
  <tr>
   <td>分數 <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>在<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">變更分數流程步驟</a>中使用此權杖。 </td>
  </tr>
  <tr>
   <td colspan="1">SFDC行銷活動 <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td>
   <td colspan="1">使用此代號，可將成為Marketo計劃一部分的潛在客戶也新增至新增的任何其他SFDC Campaign。</td>
  </tr>
  <tr>
   <td>文字 <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>只是一些文字。 當HTML過度使用它時。 文字權杖的大小限製為524,288個字元(UTF-8)或2 MB。</td>
  </tr>
 </tbody>
</table>

>[!CAUTION]
>
>在[!DNL Microsoft Dynamics]或[!DNL Salesforce]上從Sales Insight傳送電子郵件時，我的Token無法解析；只會填入標準權杖（銷售機會、公司等）。 但是，權杖&#x200B;_的預設值將_&#x200B;有效。

## 巢狀代號 {#nesting-tokens}

當您建立新的Token時，樹狀結構中的其他物件可參考它。 建立Token時所用的命名結構方便管理。

* **本機Token：**&#x200B;該Token是直接在該程式或資料夾中建立的。
* **繼承的Token：** Token是在樹狀結構上較高層級程式或資料夾中的某個位置建立的。
* **覆寫的Token：**&#x200B;已繼承Token，然後有人在此程式或資料夾中發生例外狀況。

您可以建立全域變數，然後在樹狀結構的較低層級覆寫它們。

移動程式和資料夾也會影響代號。 請務必檢查以確保在移動期間參照不會中斷。

>[!IMPORTANT]
>
>[批次行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md#batch-campaign){target="_blank"}不支援巢狀權杖。

>[!NOTE]
>
>如果您從參與計畫傳送的電子郵件是預設計畫的子電子郵件（不是您參與計畫的本機），則電子郵件中使用的任何「我的Token」都會從子電子郵件所在的預設計畫解析。

>[!MORELIKETHIS]
>
>* [Token概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [管理我的Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
