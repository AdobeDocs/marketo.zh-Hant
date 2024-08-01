---
description: 發行說明 — 2024年3月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2024 年 3 月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 1839ccb646e775b67efa8de7d2d2bf3dbbbefa72
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# 發行說明： 2024年3月 {#release-notes-mar-24}

下方提供2024年3月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2024年3月8日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
  <tr> 
   <td><strong>進階交談流程邏輯</strong>：在交談流程後續追蹤的單一選擇中，新增要評估的其他欄位。</td> 
   <td>已送出</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageForms的對話流量設定</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>重新排序對話流程邏輯</strong>：在FormsMarketo Engage中，您現在可以重新排序對話流程選擇，而不必刪除並重新新增。</td> 
   <td>已送出</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageForms的對話流量設定</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API活動中繼資料</strong>： 
   使用者代理程式、平台和裝置等中繼資料現在包含在網路和電子郵件活動中，有助於透過Marketo REST API提供這些活動的一致深入分析。</td> 
   <td>已送出</td>
   <td>不適用</td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **取得方案成員API修正**：最近已進行變更，以修正[取得方案成員](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}端點的行為。 先前，當使用`updatedAt`篩選型別來指定日期範圍時，在該範圍內更新的方案會籍記錄可能會不包含在回應中。 此外，指定日期範圍以外更新的方案會籍記錄也可能會不正確地包含在回應中。 這兩個問題都已解決。

* **帳戶分析瀏覽器外掛程式淘汰**：Adobe將於2024年4月8日從Chrome網站商店移除Target帳戶管理[帳戶分析瀏覽器外掛程式](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"}。 現有使用者：您可以繼續使用外掛程式，直到您將您的Marketo Engage執行個體移轉至Adobe身分和Admin Console為止。 此變更&#x200B;**不會影響Marketo Engage或Chrome與Outlook電子郵件外掛程式中，與Sales Insight搭配使用的任何其他TAM功能/資料**。 [了解更多](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}。
