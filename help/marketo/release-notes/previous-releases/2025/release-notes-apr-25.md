---
description: 發行說明 — 2025年4月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 4 月
feature: Release Information
exl-id: 94010780-41aa-4212-a1d4-1b78806bd728
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 37%

---

# 發行說明：2025 年 4 月 {#release-notes-apr-25}

下方提供2025年4月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年4月25日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>安全通訊端層(SSL)自助服務</strong>： SSL加密可讓您保護Marketo Engage執行個體的登入頁面。 啟用此功能過去需要Adobe支援團隊的協助。 Marketo使用者現在可以自行啟用，節省寶貴時間。</td>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-ssl-to-your-landing-pages.md">新增SSL至您的登入頁面</a></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **全新Analytics功能 — 公用Beta**： [進階BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (先前稱為Revenue Explorer和Advanced Report Builder)在4月中旬開始向所有目前的Revenue Cycle Explorer使用者推出。 這個新工具針對Marketo Engage資料提供彈性的報表和視覺化介面，提供關於進度、效能等專案的詳細資訊。 它提供更豐富的互動性和視覺效果、更快的效能，以及更順暢且直覺的使用者體驗。

若要存取此功能，您必須已購買進階BI Analytics附加元件。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

* **REST API「access_token」參數棄用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將棄用，且於 2026 年 3 月 31 日之後即不再提供。所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 棄用**：將於 2026 年 3 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **棄用社交功能**： 2024年7月31日星期三，Marketo Engage開始棄用產品中的下列社交功能：

   * 投票
   * 社交按鈕
   * 推薦優惠方案
   * 影片分享
   * 抽獎

截至目前，使用者無法在Marketo Engage中建立、複製或嵌入任何這些Social功能。 現有的社交資產可持續使用至2025年1月31日。 2025年2月1日，社交資產停止運作。 登陸頁面中內嵌的任何社交功能都將需要移除。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
