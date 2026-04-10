---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: af89a1a1fd0246564d0904103f742230a096de04
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 24%

---

# 發行說明：2026 年 3 月 {#release-notes-mar-26}

下方提供2026年3月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年3月27日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 管理品牌（測試版）</strong>：根據您組織/品牌的特定撰寫准則產生電子郵件內容。</td>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">建立和管理品牌</a></td>
  </tr>
  <tr>
   <td> </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 快速動作</strong>： <i>與舊電子郵件編輯器的對等性</i>。 快速動作現在可用於所有電子郵件Designer資產（電子郵件、電子郵件範本、片段）。 支援的快速動作包括：複製、刪除、移動、建立/編輯草稿。
   </td>
   <td>已發行</i></td>
   <td>不適用</td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
   <tr>
   <td><strong>電子郵件Designer - Outlook轉譯修正</strong>：此更新修正轉譯問題，尤其是在MS Outlook中。 進階HTML模式可讓您進行細微的HTML/CSS編輯，或新增指令碼標籤至您的電子郵件範本。
   </td>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/advanced-html-mode.md" target="_blank">使用進階HTML編輯器編輯電子郵件範本</a></td>
  </tr>
  <tr>
   <td> </td>
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
   <td><strong>挑選清單管理</strong>：您現在可以指定可以在Marketo Engage的欄位中使用的值。
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
   <td><strong>推播通知</strong>：在推播通知訊息中設定的重新導向URL現在支援Marketo Engage權杖（僅適用於<i>啟動應用程式URL</i>）。
   </td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **SEO功能淘汰**： 2026年3月31日（星期二），Marketo Engage將淘汰搜尋引擎最佳化功能(SEO)。 如果您未主動使用SEO，則不必執行任何動作。 如果您最近曾使用SEO，您可以選擇匯出資料。 [了解更多](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}。

* **REST API合併潛在客戶限制**：自2026年3月31日起，在合併潛在客戶API呼叫的leadIds引數中包含超過25個ID的呼叫將產生1080錯誤碼，該呼叫將被跳過。 需要將超過25筆記錄合併成一筆的工作應分割成多個工作，以確保這些呼叫成功。

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年7月31日後無法使用。 所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2026年7月31日終止。 使用 SOAP API 功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
