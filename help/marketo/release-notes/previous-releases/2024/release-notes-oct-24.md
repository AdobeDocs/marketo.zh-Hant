---
description: 發行說明 — 2024年10月 — Marketo檔案 — 產品檔案
title: 版本注意事項 - 2024 年 10 月
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 16%

---

# 發行說明：2024 年 10 月 {#release-notes-oct-24}

下方提供2024年10月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2024年10月4日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
    <tr>
   <td><strong>互動式網路研討會的權杖化</strong>：您現在可以使用權杖在電子郵件和登陸頁面中推廣互動式網路研討會，而無需手動新增網路研討會詳細資訊。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">推廣互動式網路研討會</a></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  </tr>
   <tr>
   <td><strong>智慧清單「設定為影響」計數</strong>：檢視編輯Smart Campaign的資格規則時會影響多少人。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  </tr>
   <tr>
   <td><strong>導覽邊欄中的「我的帳戶」按鈕</strong>：對於已移轉至Adobe Identity Management系統的使用者，左側導覽邊欄中新的「我的帳戶」按鈕可讓您設定時區並存取訂閱詳細資料。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
   <tr>
   <td><strong>電子郵件效能報告增強功能</strong>：已針對電子郵件報告量度和活動追蹤進行多項改進，以提供其他深入分析並改善準確性。
   <ul>
   <li>從電子郵件效能量度篩選刪除和合併的人員</li>
   <li>電子郵件在等待回應活動三天後現在分類為<i>已中止</i></li>
   <li>電子郵件開啟次數會計為每個Smart Campaign個別開啟的唯一開啟次數</li>
   </td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">電子郵件績效報告</a></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
   <tr>
   <td><strong>Salesforce同步處理待處理專案量度</strong>：監視同步處理輸送量和待處理專案趨勢，以便規劃及排程CRM更新，提供最佳的同步處理體驗。
   </td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Salesforce 同步待辦項目量度</a></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **大量擷取API更新**：我們已修正大量擷取API中涉及columnHeaderNames選項的問題，該選項可讓您在匯出的檔案中指定自訂欄標題名稱。 以前，包含非ASCII字元的欄標題名稱可能會損毀。

* **Rest API access_token引數淘汰**：用於驗證Marketo REST API呼叫的「access_token」查詢引數已淘汰，並將於2026年3月31日後無法使用。 所有新的和現有的整合應該使用&#39;Authorization&#39;標頭[驗證REST API呼叫，如此處所述](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token)。

* **QR碼淘汰**：自2024年10月4日起，推播通知和應用程式內訊息資產中使用的QR碼功能將被淘汰。 這包括使用新測試裝置的QR碼，以及使用QR碼建立新資產。 淘汰使用率較低的功能，可讓我們重新分配其資源，以進行Marketo Engage的整體維護。

* **Munchkin變更**

   * **新版本**：自2024年9月17日起，[Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164將開始在&#x200B;**管理員** > **Treasure Chest**&#x200B;中啟用「Munchkin Beta」設定的Marketo Engage執行個體推出。 排程在10月29日開始推出至所有其他執行個體。 此版本會更新Munchkin Cookie的建立。 功能沒有變更。

   * **已移除URL中的字元**： Munchkin JS建立的「瀏覽網頁」和「點按連結」活動現在會移除所有URL欄位中的非URL編碼控制字元。 此項變更旨在防止錯誤傳播至不支援這些字元型別，且在Marketo Engage中沒有有效使用的系統。
