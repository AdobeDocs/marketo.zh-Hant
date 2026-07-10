---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: d0cf66fe0c72af8e9d1db09792f73fd6db10abbb
workflow-type: tm+mt
source-wordcount: 477
ht-degree: 22%

---

# 發行說明： 2026年7月 {#release-notes-july-26}

以下是2026年7月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年7月10日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。 如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>Marketo AI技能 — 產品知識</strong>：產品知識可讓您隨選存取Marketo專業知識，而不需離開平台。 以簡單的語言提出問題，Marketo AI就會利用官方Adobe檔案來回答。</td>
   <td>開啟Beta版</td>
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
   <td>開啟Beta版</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">調查銷售機會</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer - AI小幫手內容功能表</strong>：現在可以從內容功能表（黑色列）存取電子郵件Designer的AI小幫手功能。 例如，當您選取文字內容時，「AI輔助程式」圖示會出現在內容功能表上，可讓您從該處執行快速動作。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年7月31日後無法使用。 所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API合併潛在客戶限制**：自2026年7月31日起，在合併潛在客戶API呼叫的leadIds引數中包含超過25個ID的呼叫將產生1080錯誤碼，並將略過該呼叫。 需要將超過25筆記錄合併成一筆的工作應分割成多個工作，以確保這些呼叫成功。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2026年7月31日終止。 使用 SOAP API 功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **取得潛在客戶活動與取得潛在客戶變更的靜態清單大小限制**：自2026年9月30日起，如果目標靜態清單包含10,000個或更多潛在客戶，呼叫Get潛在客戶活動與取得潛在客戶變更包含`listId`引數的端點將傳回1003錯誤代碼。 如需詳細資訊，請參閱[移轉指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。
