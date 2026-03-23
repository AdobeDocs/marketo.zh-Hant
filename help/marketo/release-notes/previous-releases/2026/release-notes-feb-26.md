---
description: 發行說明 — 2026年2月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2026 年 2 月
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 937c4a43066f957ddbeab9363174bc04e9a7d718
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 25%

---

# 發行說明：2026 年 2 月 {#release-notes-feb-26}

下方提供2026年2月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年2月20日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 資料夾動作</strong>：與舊的電子郵件編輯器對等。
   <ul>
   <li>共用和封存電子郵件Designer資產的資料夾動作。</li>
   <li>跨工作區共用資料夾、以滑鼠右鍵按一下資料夾以建立新資產、透過拖放方式來移動資產。</li>
   </ul>
   </td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer - API</strong>：您現在可以使用電子郵件Designer的API呼叫。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer - Brand Quality Checker</strong>：評估一般內容品質，找出可讀性、內容一致性和有效性的潛在問題，不受品牌准則影響。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer - AI助理影像產生</strong>：現在除了Firefly之外，您還可以使用Nano Banana模型，透過AI助理產生電子郵件內容的影像。</td>
   <td>已發行</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">為您的電子郵件特定區段建立內容</a></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **SEO功能淘汰**： 2026年3月31日（星期二），Marketo Engage將淘汰搜尋引擎最佳化功能(SEO)。 如果您未主動使用SEO，則不必執行任何動作。 如果您最近曾使用SEO，您可以選擇匯出資料。 [了解更多](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}。

* **REST API合併潛在客戶限制**：自2026年3月31日起，在合併潛在客戶API呼叫的leadIds引數中包含超過25個ID的呼叫將產生1080錯誤碼，該呼叫將被跳過。 需要將超過25筆記錄合併成一筆的工作應分割成多個工作，以確保這些呼叫成功。

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年7月31日後無法使用。 所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2026年7月31日終止。 使用 SOAP API 功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
