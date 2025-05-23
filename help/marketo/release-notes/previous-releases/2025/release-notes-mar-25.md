---
description: 發行說明 — 2025年3月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 3 月
feature: Release Information
exl-id: a0e45d8e-6b74-4ab0-a1ba-4dae3754bc8f
source-git-commit: f236f2cf73637ee1a0ee6062c1ecbf82f0e02130
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 3%

---

# 發行說明： 2025年3月 {#release-notes-mar-25}

下方提供2025年3月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

您可在此處[&#128279;](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到Adobe Dynamic Chat 專屬的發行說明。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年3月28日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
    <tr> 
   <td><strong>所有程式都可使用Designer電子郵件</strong>：參與、預設和事件程式現在都可存取新的Designer電子郵件（互動式網路研討會程式除外）。 以前它們只能用於電子郵件計畫。</td>
   <td>已送出</td>
   <td>不適用</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>互動式網路研討會中的GenAI功能</strong>：您現在可以產生章節以及隨選網路研討會的摘要。 編輯並匯出資料的HTML檔案。</td>
   <td>已送出</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai">GenAI功能</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>全域與Workspace My Token</strong>：在工作區與全域層級設定我的Token，以提升生產力並控制Marketo Engage工作區乃至整個執行個體的品牌與行銷宣傳資料。</td> 
   <td>已送出</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md#create-a-my-token">建立全域「我的Token」</a></td>
  </tr>
  </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **棄用社交功能**： 2024年7月31日星期三，Marketo Engage開始棄用產品中的下列社交功能：

   * 投票
   * 社交按鈕
   * 推薦人特賣優惠
   * 影片分享
   * 抽獎

截至目前，使用者無法在Marketo Engage中建立、複製或嵌入任何這些Social功能。 現有的社交資產可持續使用至2025年1月31日。 2025年2月1日，社交資產停止運作。 登陸頁面中內嵌的任何社交功能都將需要移除。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2025年10月31日後無法使用。 所有新的和現有的整合應該使用&#39;Authorization&#39;標頭[驗證REST API呼叫，如此處所述](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2025年10月31日終止。 使用SOAP API功能的服務應移轉至[REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **全新Analytics功能 — 公用Beta**： [進階BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (先前稱為Revenue Explorer和Advanced Report Builder)在4月中旬開始向所有目前的Revenue Cycle Explorer使用者推出。 這個新工具針對Marketo Engage資料提供彈性的報表和視覺化介面，提供關於進度、效能等專案的詳細資訊。 它提供更豐富的互動性和視覺效果、更快的效能，以及更順暢且直覺的使用者體驗。

若要存取此功能，您必須已購買進階BI Analytics附加元件。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。
