---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 978bbe4de06a0e269b60108e5a91edc5499dc9c1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 3%

---

# 版本說明：2025 年 3 月 {#release-notes-mar-25}

您將在下面找到 March &#39;25 版本中包含的所有功能。 請查看您的 Adobe Systems Marketo Engage 版以瞭解功能可用性。

可以在此處](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到Adobe Systems動態聊天[的發行說明。

>[!AVAILABILITY]
>
>用星號（星號](assets/yellow-star.png)）![表示的功能是付費附加元件。請聯繫您的Marketo Engage代表以瞭解更多資訊。

## 標準發佈週期功能 {#standard-release-cycle-features}

以下功能屬於標準發佈週期，開始於 2025 **年 3 月 28 日**&#x200B;發佈，並在隨後幾周內分階段轉出剩餘功能。發行功能和日期可能會有所變更。 請檢查每個功能旁邊的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
    <tr> 
   <td><strong>電子郵件設計器可用於所有計劃</strong>：新 電子郵件設計器電子郵件現在可以跨參與、預設和活動計劃訪問（互動式網路研討會計劃是唯一例外）。 以前，它們只能在電子郵件程式中使用。 在此更新中，克隆也變得可用。</td>
   <td>運</td>
   <td>不適用</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>互動式網路研討會</strong>中的 GenAI 功能：您現在可以為點播網路研討會生成章節和摘要。 編輯並導出数据的 HTML 文件。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>全域和工作環境我的令牌</strong>：在工作環境和全域級別配置我的令牌，以提高工作效率並跨Marketo Engage工作區和平均整個實例控制品牌和行銷抵押品。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>任何觸發器屬性</strong>的令牌：從此文件中的 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments" target="_blank">清單擴展可用觸發令牌清單</a> ，以支持在行銷活動流字段中使用任何觸發活動屬性中的數據。 列印活動属性中的數據到有趣的時刻，或將自定義活動中銷售機會的最新交易 ID 設置到銷售機會字段中。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **Social功能棄用**：2024 年 7 月 31 日星期三，Marketo Engage 開始棄用產品中的以下Social功能：

   * 民意調查
   * Social按鈕
   * 推薦人特賣優惠
   * 影片分享
   * 抽獎

截至那時，用戶無法在Marketo Engage中創建、克隆或嵌入任何這些Social功能。 現有Social資產會持續運作到 2025 年 1 月 31 日。 2025年2月1日，Social資產停止運作。 登陸頁面中嵌入的任何社交功能均需予以移除。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Rest API「access_token」參數棄用**： `access_token` 用於驗證 Marketo REST API 呼叫的 查詢 參數即將棄用，2025 年 6 月 30 日之後將無法使用。 如此處](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}所述，[所有新的和現有的整合都應使用「授權」標頭對 REST API 呼叫進行身份驗證。

* **SOAP API 淘汰**：對 Marketo SOAP API 的支援將於 2025 年 10 月 31 日終止。 使用SOAP API功能的服務應遷移至 [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **新 Analytics 功能 - 公共Beta**： [進階 BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} （以前稱為收入資源管理員和進階 Report Builder）將於 4 月中旬開始向所有當前的收入周期資源管理器使用者推出。 這個新工具為Marketo Engage數據提供了一個靈活的報告和可視化介面，提供有關進度、性能等的粒度詳細信息。 它具有更豐富的互動和可視化效果、更快的性能以及更無縫、更直觀的使用者體驗。

若要存取此功能，您必須已購買 進階 BI Analytics 附加元件。 請洽詢 Adobe Systems 客戶團隊（您的客戶經理）以取得詳細資訊。
