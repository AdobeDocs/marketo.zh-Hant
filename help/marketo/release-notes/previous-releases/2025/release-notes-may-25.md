---
description: 發行說明 — 2025年5月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 5 月
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 33%

---

# 發行說明：2025 年 5 月 {#release-notes-may-25}

以下是2025年5月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年5月23日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件Designer Assets的角色型存取控制</strong>：角色型存取控制(RBAC)系統的新增強功能，提供更精細的許可權，並改善新電子郵件Designer所支援的資產使用者管理。</td>
   <td>已發行</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">新電子郵件Designer的精細許可權（部落格）</a></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>複製在電子郵件Designer中建立的電子郵件</strong>：您現在可以複製使用新電子郵件Designer建立的現有電子郵件。</td>
   <td>已發行</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>任何屬性的觸發權杖</strong>：擴充的觸發權杖清單，可支援在Smart Campaign欄位中使用任何活動屬性的資料。</td>
   <td>已發行</td>
   <td>不適用</td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Facebook離線轉換整合更新**：在2025年5月29日，Marketo Engage的[Facebook離線轉換](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"}整合將移轉到新的Meta [轉換API](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}，因為Meta已依照Graph API版本設定棄用[離線轉換API](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"}。 如需詳細資訊，請檢視Meta的[透過轉換API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} （離線的CAPI）傳送離線事件的指南。

* **全新Analytics功能 — 公用Beta**： [進階BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (先前稱為Revenue Explorer和Advanced Report Builder)已於4月中旬開始向所有目前的Revenue Cycle Explorer使用者推出。 這個新工具針對Marketo Engage資料提供彈性的報表和視覺化介面，提供關於進度、效能等專案的詳細資訊。 它提供更豐富的互動性和視覺效果、更快的效能，以及更順暢且直覺的使用者體驗。

若要存取此功能，您必須已購買進階BI Analytics附加元件。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

* **REST API「access_token」參數棄用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將棄用，且於 2026 年 3 月 31 日之後即不再提供。所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 棄用**：將於 2026 年 3 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
