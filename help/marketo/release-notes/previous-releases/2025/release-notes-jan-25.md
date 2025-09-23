---
description: 發行說明 — 2025年1月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 1 月
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 23%

---

# 發行說明：2025 年 1 月 {#release-notes-jan-25}

以下是2025年1月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年1月17日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
    <tr>
   <td><strong>新電子郵件Designer</strong>：使用Marketo Engage中的新原生電子郵件Designer，建立現代且有效的電子郵件。 存取其中一個預先設計的現成電子郵件範本，或輕鬆建立您自己的範本。 使用動態內容並從Adobe Experience Manager雲端服務存取影像。 使用Content Accelerator Gen-AI功能，大規模建立創新且高效能的電子郵件。
   <p><img src="assets/note-icon.png" alt="附註圖示"> 注意：若要存取新的電子郵件設計工具，您的Marketo Engage訂閱必須移轉至<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management系統(IMS)</a>。 如果尚未收到您的邀請，而您想要請求加急，請聯絡Adobe客戶團隊（您的客戶經理）或<a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo支援</a>。 若要存取Content Accelerator Gen-AI功能，請聯絡Adobe客戶團隊。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">電子郵件設計工具概觀</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>在互動式網路研討會中取消註冊註冊者</strong>：現在，如果您由於任何原因不想讓註冊者參加網路研討會，可以取消註冊。 工作流程會從Marketo事件計畫和Adobe Connect中移除註冊者。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>停用封存的行銷活動</strong>：停用作用中觸發行銷活動，並在封存時取消資料夾中行銷活動的任何排程批次執行。 由於對包含有效行銷活動的封存資料夾有額外的許可權檢查（啟用觸發行銷活動和排程批次行銷活動），因此此功能在此版本中預設為停用，並可在您的Marketo Engage訂閱中導覽至<b>管理員</b> &gt; <b>Treasure Chest</b>來啟用。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **棄用社交功能**： 2024年7月31日星期三，Marketo Engage開始棄用產品中的下列社交功能：

   * 投票
   * 社交按鈕
   * 推薦優惠方案
   * 影片分享
   * 抽獎

截至目前，使用者無法在Marketo Engage中建立、複製或嵌入任何這些Social功能。 現有的社交資產可持續使用至2025年1月31日。 在2025年2月1日，社交資產將停止運作。 需要移除內嵌在登陸頁面中的社交功能。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **取得方案成員API更新**：我們已增強[取得方案成員](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} API以支援擷取方案成員識別碼的功能。 做法是將ID新增至API請求的欄位引數中指定的欄位清單中。

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年1月31日後無法使用。 所有新的和現有的整合都應使用「授權」標頭驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2026年1月31日終止。 使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
