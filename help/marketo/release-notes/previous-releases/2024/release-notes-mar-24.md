---
description: 發行說明 — 2024年3月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2024年3月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 發行說明： 2024年3月 {#release-notes-mar-24}

下方提供2024年3月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![星形](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於以下日期開始發行 **2024年3月8日**，在接下來的幾週內分階段推出剩餘的功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
  <tr> 
   <td><strong>進階對話流程邏輯</strong>：新增其他欄位以供在單一選擇中進行評估，以進行交談流量追蹤。</td> 
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
   <td><strong>重新排序對話流程邏輯</strong>：在Marketo EngageForms中，您現在可以重新排序對話流程選擇，而不必刪除並重新新增。</td> 
   <td>已送出</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageForms的對話流量設定</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API活動中繼資料</strong>：中繼資料（例如使用者代理、平台和裝置）現在包含在網路和電子郵件活動中，有助於透過Marketo REST API提供這些活動的一致深入分析。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **取得方案成員API修正**：最近已進行變更以修正的行為 [取得計畫成員](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"} 端點。 先前，當使用 `updatedAt` 篩選型別若要指定日期範圍，回應中可能會不包含在該範圍內更新的方案會籍記錄。 此外，指定日期範圍以外更新的方案會籍記錄也可能會不正確地包含在回應中。 這兩個問題都已解決。

* **帳戶分析瀏覽器外掛程式淘汰**：Adobe正在移除Target帳戶管理 [帳戶分析瀏覽器外掛程式](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} 於2024年4月8日在Chrome線上應用程式商店買賣。 現有使用者：您可以繼續使用外掛程式，直到您將您的Marketo Engage執行個體移轉至Adobe身分和Admin Console為止。 此變更 **將不會影響** Marketo Engage內的任何其他TAM功能/資料，或搭配Sales Insight使用的Chrome和Outlook電子郵件外掛程式。 [瞭解更多](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
