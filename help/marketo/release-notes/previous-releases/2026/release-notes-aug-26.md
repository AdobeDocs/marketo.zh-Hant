---
description: 發行說明 — 2026年7月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2026年7月
feature: Release Information
source-git-commit: a1b00f94acf0fe9cd354a48bf40f17c3ad9b8ae6
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 13%
---
# 發行說明： 2026年8月 {#release-notes-aug-26}

下方提供2026年8月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年8月14日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。 請查看各項功能旁邊的狀態。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>Marketo Engage全新UI</strong>： Marketo Engage介面具有重新整理的外觀，包括更新的功能表、圖示和版面，可提供更乾淨、更現代的體驗。 這僅是視覺化更新；不影響現有功能或工作流程。
</td>
   <td>在8月和9月期間分階段推出</td>
   <td><i>不適用</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo Engage MCP伺服器</strong>： Marketo Engage MCP伺服器可做為您AI助理與Marketo Engage之間的橋樑。 它會公開超過100項操作，涵蓋表單、方案、智慧行銷活動、人員/銷售機會、電子郵件、代碼片段、清單和資料夾。</td>
   <td>現已正式推出</td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/mcp-server.html?lang=zh-Hant" target="_blank">Marketo MCP伺服器</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>停用封存的行銷活動</strong>：封存資料夾現在會停用並取消排程該資料夾樹狀結構中的所有行銷活動，防止未預期地執行封存的智慧行銷活動。
</td>
   <td>已發行</td>
   <td><a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders#disable-campaigns-archive" target="_blank">在封存上停用行銷活動</a></td>
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
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo AI現在是Marketo Engage的同事了**： Marketo Engage的同事提供了代理程式技能，可自動執行耗時的行銷功能。 新名稱、相同功能，可供所有使用者使用。 [了解更多](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **REST API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年8月31日後無法使用。 所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API行銷活動執行ID**：在某些情況下，活動的行銷活動執行ID值有時會在兩對引號（例如`"campaignRunId": ""102938""`）之間，以不正確的格式傳回。<br/>從8月發行版本開始，此值一律會以正確的數字格式(`"campaignRunId": 102938`)傳回

* **取得潛在客戶活動與取得潛在客戶變更的靜態清單大小限制**：自2026年9月30日起，如果目標清單包含10,000個或更多潛在客戶，呼叫Get Lead活動或包含`listId`引數的Get Lead Changes端點會失敗，並產生1003錯誤碼（表示目標靜態清單有太多記錄）。 如需詳細資訊，請參閱[移轉指南](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。

* **REST API合併潛在客戶限制**：自2026年7月31日起，在合併潛在客戶API呼叫的leadIds引數中包含超過25個ID的呼叫會產生1080錯誤碼，並略過該呼叫。 需要將超過25筆記錄合併成一筆的工作應分割成多個工作，以確保這些呼叫成功。
