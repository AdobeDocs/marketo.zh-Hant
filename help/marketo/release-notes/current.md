---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6b9f6d4b276115e1f3f3dac73eb64e5358a76516
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 99%

---

# 發行說明：2025 年 10 月 {#release-notes-oct-25}

以下為 2025 年 10 月發行版本中包含的所有功能。請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

以下功能屬於標準發行週期，並且將於 **2025 年 10 月 31 日**&#x200B;開始發行，其餘功能則會在接下來數週內分階段推出。發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 範本匯入工具 (Beta)</strong>：從傳統電子郵件編輯器匯入電子郵件範本，來建立與 Design Studio 中新電子郵件設計工具相容的範本。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">範本匯入</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 條件式內容</strong>：新電子郵件設計工具的同等功能，可讓您在權杖之外實現電子郵件個人化。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/conditional-content.md" target="_blank">條件式內容</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>電子郵件設計工具 - 影像轉 HTML 轉換器</strong>：上傳電子郵件相容的 PNG/JPEG 影像檔案，此檔案會自動轉換為 HTML，以便用於新電子郵件設計工具。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/image-to-html.md" target="_blank">將影像轉換為HTML範本</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 原地複製電子郵件動作</strong>：您現在可以將電子郵件原地複製至行銷活動中另一個計劃的資料夾，並快速重複使用現有的電子郵件。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - A/B 測試</strong>：新電子郵件設計工具的同等功能，可讓您執行 A/B 測試，藉此查看哪些類型的內容接收最佳回應。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 品牌主題</strong>：您現在可以在 Marketo Engage 中定義品牌主題。樣式設定可以在電子郵件範本和其他電子郵件資產中重複使用及套用，以維持品牌一致性。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Salesforce CRM 整合升級**：原生 CRM 整合的新版本自 2025 年 11 月 13 日起的七日內，將部署至已啟用原生連接器的主要沙箱。在[此 Nation 貼文](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}中取得完整詳細資訊

* **REST API 雙斜線棄用**：在 2025 年 9 月 16 日，Adobe 已轉換至更現代化的 REST API URL 託管基礎結構，採用更新的技術，增加安全性和擴充性。如果您的訂閱在 URL 中使用具有雙正斜線 (//) 的 API，請閱讀[此 Nation 文章](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"}，以了解後續步驟。

* **在新的電子郵件設計工具中切換回 Velocity 指令碼**：Adobe Marketo Engage 於今年 6 月針對新的電子郵件設計工具發布了一項稱為&#x200B;_條件式內容_&#x200B;的功能。此功能之前是由 Handlebar 指令碼而不是 Velocity 指令碼提供支援，以在您的動態內容中提供更多靈活度。但是，當我們發現它導致部分權杖發生錯誤解析時，我們就決定暫時停用。[了解更多](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity 終止服務**：2025 年 8 月，Adobe 已開始逐步停止對於 Marketo Engage Identity (透過 `login.marketo.com` 登入) 的支援。為避免 Marketo Engage 的存取中斷，您最晚必須在 2025 年 9 月 30 日轉換至 [Adobe Identity](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _IP 限制棄用_：已於 2025 年 7 月 30 日停止支援「[根據 IP 限制 Marketo 登入](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}」的功能。此功能將保持正常運作，直到轉換至 Adobe Identity 的作業完成為止。Adobe Admin Console 中即將推出適用於 Adobe Identity 的全新位置型存取控制功能。

   * _單一登入 (SSO) 棄用_：已於 2025 年 7 月 30 日停止支援 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}。該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。在 Adobe Admin Console 中，Adobe Identity 單一登入必須個別設定。關於設定步驟，請參閱[設定身分識別和單一登入](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

* **棄用「_轉寄給好友_」功能**：自 2025 年 9 月 29 日起，Marketo Engage 2.0 電子郵件 (舊版電子郵件編輯器) 中的「_轉寄給好友_」功能在所有訂閱中已全面棄用。此變更影響已寄出或即將寄出，且使用「轉寄給好友」權杖的電子郵件中的「轉寄給好友」權杖和連結。[了解更多](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **REST API「access_token」參數棄用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將棄用，且於 2026 年 1 月 31 日之後不再提供使用。所有新的和現有的整合都應使用「授權」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 棄用**：將於 2026 年 1 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
