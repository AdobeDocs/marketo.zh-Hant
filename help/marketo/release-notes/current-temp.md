---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 47%

---

# 發行說明：2026 年 1 月 {#release-notes-jan-26}

以下是2026年1月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2026年1月30日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>功能標題</strong>：功能說明。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>功能標題</strong>：功能說明。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td>  </td>
   <td>  </td>
   <td>  </td>
  </tr>
  <tr>
   <td><strong>功能標題</strong>：功能說明。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Adobe Connect功能 {#adobe-connect-features}

Marketo Engage [互動式網路研討會](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"}功能由Adobe Connect提供技術支援，透過事件資料豐富人員管理和行銷活動，並提升人員品質。 以下是一些直接影響互動式網路研討會使用者的最新Adobe Connect版本。

* **調查Pod**： Adobe Connect 12.11推出新的Survey Pod，讓主機直接在即時工作階段中設計和傳遞結構化意見表單。

* **資源Pod**：新的資源Pod會取代先前的檔案和Web連結Pod，提供在即時工作階段中共用資源的單一統一方式。

* **增強型房間介面體驗**： Adobe Connect 12.11採用更新且更現代的房間介面，建構在Adobe最新的Spectrum 2設計架構上，與其他Adobe產品(例如Creative Cloud和Experience Cloud)所使用的視覺語言一致。

如需完整詳細資訊，請檢閱[Adobe Connect 12.11發行說明](https://helpx.adobe.com/tw/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}。

## 公告 {#announcements}

* **Rest API &#39;access_token&#39;引數淘汰**：用於驗證Marketo REST API呼叫的`access_token`查詢引數已淘汰，並將於2026年3月31日後無法使用。 所有新的和現有的整合都應使用「授權」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API淘汰**：對Marketo SOAP API的支援將於2026年3月31日終止。 使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **Marketo Engage身分服務終止**：

   * _IP 限制棄用_：已於 2025 年 7 月 30 日停止支援「[根據 IP 限制 Marketo 登入](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}」的功能。此功能將保持正常運作，直到轉換至 Adobe Identity 的作業完成為止。Adobe Admin Console 中即將推出適用於 Adobe Identity 的全新位置型存取控制功能。

   * _單一登入 (SSO) 棄用_：已於 2025 年 7 月 30 日停止支援 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}。該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。在 Adobe Admin Console 中，Adobe Identity 單一登入必須個別設定。關於設定步驟，請參閱[設定身分識別和單一登入](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。
