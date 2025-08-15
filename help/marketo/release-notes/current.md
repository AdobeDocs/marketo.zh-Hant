---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 46%

---

# 發行說明：2025 年 8 月 {#release-notes-aug-25}

下方提供2025年8月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否適用這些功能。

Adobe Dynamic Chat 特定的發行說明[請參閱此處](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2025年8月22日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。各項功能的狀態請查看旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 報告</strong>：電子郵件效能和電子郵件連結效能報告現在會顯示使用新電子郵件Designer建立的電子郵件資料。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 電子郵件預覽最佳化</strong>：某些使用者嘗試在電子郵件/電子郵件範本/片段詳細資訊頁面中預覽其電子郵件時，載入時間會變慢。 此體驗已最佳化，載入時間最多可加快60%。</td>
   <td><i>即將推出</i></td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 範本修正</strong>：部分現成範本發生轉譯問題(例如，在某些瀏覽器/深色模式中無法正確轉譯、影像未對齊、CTA按鈕放置錯誤，以及更多問題)。 此版本已修正所有問題。</td>
   <td><i>即將推出</i></td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 內容鎖定修正</strong>：以前，如果電子郵件範本是以內容鎖定方式建立，且範本是用來建立電子郵件，則即使電子郵件已重設或選取「變更設計」，內容鎖定也會持續存在。 此問題已在此版本中修正。</td>
   <td><i>即將推出</i></td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件Designer — 自動完成移除</strong>：權杖個人化編輯器中的自動完成選項指向錯誤的物件，因此已移除。 目前沒有重新實作它的計畫。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo Engage Identity生命週期結束**：自2025年8月起，Adobe開始逐步停止支援Marketo Engage Identity （透過`login.marketo.com`登入）。 為避免 Marketo Engage 的存取中斷，您最晚必須在 2025 年 9 月 30 日轉換至 [Adobe Identity](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _不再使用IP限制_：支援[根據IP限制Marketo登入](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}已於2025年7月30日結束。 該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。Adobe Admin Console中適用於Adobe Identity的全新位置型存取控制功能即將推出。

   * _單一登入(SSO)淘汰_：對[Marketo身分識別SSO](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}的支援已於2025年7月30日結束。 該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。在 Adobe Admin Console 中，Adobe Identity 單一登入必須個別設定。關於設定步驟，請參閱[設定身分識別和單一登入](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

* **REST API「存取權杖」參數停止適用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將停止適用，且於 2025 年 10 月 31 日之後不再提供使用。所有新的和現有的整合都應使用「授權」標頭驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 停止適用**：將於 2025 年 10 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
