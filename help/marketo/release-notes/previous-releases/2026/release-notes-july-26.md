---
description: 發行說明 — 2026年7月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2026年7月
feature: Release Information
source-git-commit: 37ef6b0f6c89b8ec8cd098beb5cf4d321fdac401
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 20%

---

# 發行說明： 2026年7月 {#release-notes-july-26}

以下是2026年7月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年7月10日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。 請查看各項功能旁邊的狀態。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>Marketo AI技能 — 產品知識</strong>：產品知識可讓您隨選存取Marketo專業知識，而不需離開平台。 以簡單的語言提出問題，Marketo AI就會利用官方Adobe檔案提供答案。
</td>
   <td>已發行</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">產品知識</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo AI技能 — 調查銷售機會</strong>：瞭解為什麼特定人員/銷售機會未達到里程碑（例如MQL、方案資格或促銷活動），並取得所發生情況的直白語言說明。
</td>
   <td>已發行</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">調查銷售機會</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 模組</strong>：您現在可以存取現成可用的完整結構化內容區塊，以加速電子郵件組合。</td>
   <td>已發行</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-modules.md" target="_blank">在電子郵件設計工具中使用模組</a></td>
  </tr>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 產生內容內容功能表</strong>：現在可以從內容功能表（黑色列）存取電子郵件Designer的「產生內容」功能。 例如，當您選取文字內容時，「產生內容」圖示會出現在內容功能表上，可讓您執行快速動作。</td>
   <td><i>即將推出</i></td>
<td><i>即將推出</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年8月31日後無法使用。 所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。
* **REST API合併潛在客戶限制**：自2026年7月31日起，在合併潛在客戶API呼叫的leadIds引數中包含超過25個ID的呼叫將產生1080錯誤碼，並將略過該呼叫。 需要將超過25筆記錄合併成一筆的工作應分割成多個工作，以確保這些呼叫成功。
* **SOAP API淘汰**：對Marketo SOAP API的支援將於2026年7月31日終止。 使用 SOAP API 功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
* **取得潛在客戶活動與取得潛在客戶變更的靜態清單大小限制**：自2026年9月30日起，如果目標靜態清單包含10,000個或更多潛在客戶，呼叫Get潛在客戶活動與取得潛在客戶變更包含`listId`引數的端點將傳回1003錯誤代碼。 如需詳細資訊，請參閱[移轉指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。
