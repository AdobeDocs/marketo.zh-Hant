---
description: 發行說明 — 2025年7月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 7 月
feature: Release Information
exl-id: 86776722-c640-4e55-9551-38ff34de566b
source-git-commit: bd1179a632c0363d62e262cb153b8f83dc0bfbf5
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 98%

---

# 發行說明：2025 年 7 月 {#release-notes-july-25}

以下為 2025 年 7 月發行版本中包含的所有功能。請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

以下功能屬於標準發行週期，將於 **2025 年 7 月 11 日**&#x200B;開始發行，其餘功能則會在接下來數週內分階段推出。發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - GenStudio 整合</strong>：在電子郵件內整合 GenStudio for Performance Marketing，提高行銷效率並維持品牌一致性。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/genstudio.md">GenStudio 與 Marketo Engage 的整合</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 自訂 CSS</strong>：現在，您在設計電子郵件時，可以在電子郵件設計工具中直接新增自訂 CSS。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/custom-css.md">將自訂 CSS 新增至您的電子郵件內容</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 使用 SpamAssassin 偵測垃圾郵件</strong>：您可以使用 Marketo Engage 中的 SpamAssassin 來測試電子郵件內容，了解 ISP/信箱提供者將其標記為垃圾郵件的可能性。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/spam-report.md">垃圾郵件報告</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 支援移動資產與方案刪除</strong>：在不同的方案之間快速搬動電子郵件資產。您現在也可以刪除包含有新的設計工具電子郵件資產的方案。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - Firefox 支援</strong>：Mozilla Firefox 現已完全支援電子郵件設計工具。若要實現最佳體驗，請務必維持瀏覽器的最新狀態。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 從屬性頁面模擬內容</strong>：利用<i>電子郵件屬性</i>模擬電子郵件資產的內容，但不需要返回編輯畫面。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 資產的角色型存取控制</strong>：5 月發行版本已針對編輯、核准和刪除權限實施角色型存取控制 (RBAC)。此版本現在提供讀取權限。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 編輯已發佈電子郵件的電子郵件屬性</strong>：即使在電子郵件發佈之後也能編輯<i>電子郵件屬性</i>。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 選取品牌化網域和網域 IP 設定</strong>：您現在可以針對每項電子郵件資產選取一個「品牌網域」和「網域 IP 設定」。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>REST API 錯誤代碼通知更新</strong>：應用程式內通知新增兩類 REST API 錯誤：606 - 超出最大速率限制，和 607 - 已達到每日配額。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>在欄位管理中顯示方案會員標準欄位</strong>：現在<i>欄位管理</i>中可以看見標準和自訂兩種方案會員欄位。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>欄位管理中的 REST API 名稱</strong>：此更新允許管理員查看 REST API 欄位名稱，但不需要匯出清單。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>可以檢視 Munchkin Cookie 和 ECID</strong>：現在於<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page">人員詳細資料頁面</a>的「資訊」索引標籤中可以看到 Munchkin Cookie 和 ECID (Experience Cloud 身分識別) 號碼清單，降低依賴 API 呼叫獲取該資訊的程度。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo Engage Identity 終止服務**：2025 年 8 月，Adobe 將開始逐步停止對於 Marketo Engage Identity (透過 `login.marketo.com` 登入) 的支援。為避免 Marketo Engage 的存取中斷，您最晚必須在 2025 年 9 月 30 日轉換至 [Adobe Identity](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _IP 限制棄用_：將於 2025 年 7 月 30 日停止支援「[根據 IP 對 Marketo 登入進行限制](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}」的功能。該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。Adobe Admin Console 將為 Adobe Identity 提供全新的位置型存取控制功能，預定於 2025 年 8 月發行。

   * _單一登入 (SSO) 棄用_：將於 2025 年 7 月 30 日停止支援 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}。該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。在 Adobe Admin Console 中，Adobe Identity 單一登入必須個別設定。關於設定步驟，請參閱[設定身分識別和單一登入](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

* **REST API「存取權杖」參數棄用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將停止適用，且於 2025 年 10 月 31 日之後不再提供使用。所有新的和現有的整合都應使用「授權」標頭驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 棄用**：將於 2025 年 10 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
