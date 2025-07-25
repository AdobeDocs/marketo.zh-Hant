---
description: 發行說明 — 2025年5月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 5 月
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 0297260b69c8573445c1f727a94f308138ee2895
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

---

# 發行說明： 2025年5月 {#release-notes-may-25}

以下是2025年5月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

您可在此處[找到Adobe Dynamic Chat ](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}專屬的發行說明。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年5月23日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody>
 <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr> 
   <td><strong>電子郵件Designer Assets的角色型存取控制</strong>：角色型存取控制(RBAC)系統的新增強功能，提供更精細的許可權，並改善新電子郵件Designer所支援的資產使用者管理。</td> 
   <td>已送出</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">新電子郵件Designer的精細許可權（部落格）</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>複製在電子郵件Designer中建立的電子郵件</strong>：您現在可以複製使用新電子郵件Designer建立的現有電子郵件。</td> 
   <td>已送出</td>
   <td>不適用</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>任何屬性的觸發權杖</strong>：擴充的觸發權杖清單，可支援在Smart Campaign欄位中使用任何活動屬性的資料。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **Facebook離線轉換整合更新**：在2025年5月29日，Marketo Engage的[Facebook離線轉換](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"}整合將移轉到新的中繼資料[轉換API](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}，因為中繼資料已棄用[離線轉換API](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"}，與Graph API版本設定一致。 如需詳細資訊，請檢視Meta的指南，以[透過Conversions API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI for Offline)傳送離線事件。

* **全新Analytics功能 — 公用Beta**： [進階BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (先前稱為Revenue Explorer和Advanced Report Builder)已於4月中旬開始向所有目前的Revenue Cycle Explorer使用者推出。 這個新工具針對Marketo Engage資料提供彈性的報表和視覺化介面，提供關於進度、效能等專案的詳細資訊。 它提供更豐富的互動性和視覺效果、更快的效能，以及更順暢且直覺的使用者體驗。

若要存取此功能，您必須已購買進階BI Analytics附加元件。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2025年10月31日後無法使用。 所有新的和現有的整合應該使用&#39;Authorization&#39;標頭[驗證REST API呼叫，如此處所述](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2025年10月31日終止。 使用SOAP API功能的服務應移轉至[REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
