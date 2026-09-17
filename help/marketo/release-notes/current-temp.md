---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ba06d7ce62da1ceb3f696527532975622e06fa70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 18%
---
# 發行說明： 2026年9月 {#release-notes-sep-26}

下方提供2026年9月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年9月25日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。 請查看各項功能旁邊的狀態。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>Marketo Engage全新UI</strong>： Marketo Engage介面具有重新整理的外觀，包括更新的功能表、圖示和版面，可提供更乾淨、更現代的體驗。 這僅是視覺化更新；不影響現有功能或工作流程。 <i>在2027年1月發行版本中將提供選取傳統UI的功能</i>。
</td>
   <td>9月底全面發佈</td>
   <td><i>不適用</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>在匯入時選取分割區</strong>：現在當您在已啟用工作區與分割區的環境中匯入人員記錄時，可以從本機工作區的分割區清單中選取。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>CRM同步處理即時通知</strong>：訂閱CRM通知的使用者，將會在其原生CRM同步處理變更的啟用狀態時收到立即通知，讓管理員更能瞭解其CRM同步處理狀態。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>自助流程步驟 — 回呼逾時增加</strong>：自助流程步驟的回呼逾時期間正從1小時增加到4小時。 您這端不需要執行任何動作。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 表格</strong>：您現在可以將內容型別「表格」拖放到電子郵件中，並可設定欄和列數。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **自訂活動屬性的API名稱限制**：透過API或UI建立的自訂活動屬性的API名稱現在只能包含英數字元和底線，而且必須以英數字元開頭。

* **取得潛在客戶活動與取得潛在客戶變更的靜態清單大小限制**：自2026年9月30日起，如果目標清單包含10,000個或更多潛在客戶，呼叫Get Lead活動或包含`listId`引數的Get Lead Changes端點會失敗，並產生1003錯誤碼（表示目標靜態清單有太多記錄）。 如需詳細資訊，請參閱[移轉指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。

* **REST API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數自2026年8月31日起已淘汰。 所有新的和現有的整合都應使用「Authorization」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API行銷活動執行ID**：在某些情況下，活動的行銷活動執行ID值有時會在兩對引號（例如`"campaignRunId": ""102938""`）之間以不正確的格式傳回。<br/>自8月發行版本起，此值一律會以正確的數字格式(`"campaignRunId": 102938`)傳回。

* **棄用從網頁抓取影像**：為了符合現代安全性和隱私權的最佳實務，從10月發行版本起，[從網頁抓取影像](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}功能將被棄用。
