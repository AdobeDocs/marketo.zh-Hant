---
description: 最新發行說明 - Marketo 文件 - 產品文件
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 77008ff8d8f7c577f48b508737e1b8eb2ac1e5ce
workflow-type: ht
source-wordcount: '653'
ht-degree: 100%

---

# 發行說明：2025 年 9 月 {#release-notes-sep-25}

以下為 2025 年 9 月發行版本中包含的所有功能。請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

以下功能屬於標準發行週期，且將於 **2025 年 9 月 19 日**&#x200B;開始發行，其餘功能則會在接下來數週內分階段推出。發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>隨選網路研討會活動保留</strong>：互動式網路研討會使用者現在可使用隨選網路研討會儀表板資料 30 天以上 (之前是只能從網路研討會當日起最多 30 天)。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 內容共同作業工作流程</strong>：您現在可以在電子郵件資產中進行註解，以及與其他 Marketo 使用者共同作業。標記團隊成員 (具有適當資產權限的 Marketo 使用者) 後，他們將收到電子郵件或即時簡短通知。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - AI 助理權限</strong>：Marketo 管理員可以為特定使用者提供生成式 AI 功能的存取權。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/ai-assistant.md#set-up-permissions">設定權限</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 深色模式</strong>：您現在可以使用深色模式，讓支援的電子郵件用戶端和應用程式以較深色的背景顯示電子郵件，並以較淺的顏色顯示文字、按鈕及其他 UI 元素。</td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md">深色模式</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 重新導向修正</strong>：部分使用者在使用這項新的設計工具建立電子郵件時，遇到 URL 重新導向的問題 (例如有時無法直接貼上 URL 或將電子郵件資產加入書籤)。此問題已解決。此外，從「<b>電子郵件範本</b>」&gt;「<b>詳細資料</b>」&gt;「<b>使用者</b>」的電子郵件資產連結，將重新導向至對應的電子郵件資產。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **在新的電子郵件設計工具中切換回 Velocity 指令碼**：Adobe Marketo Engage 於今年 6 月針對新的電子郵件設計工具發布了一項稱為&#x200B;_條件式內容_&#x200B;的功能。此功能之前是由 Handlebar 指令碼而不是 Velocity 指令碼提供支援，以在您的動態內容中提供更多靈活度。但是，當我們發現它導致部分權杖發生錯誤解析時，我們就決定暫時停用。[了解更多](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity 終止服務**：2025 年 8 月，Adobe 已開始逐步停止對於 Marketo Engage Identity (透過 `login.marketo.com` 登入) 的支援。為避免 Marketo Engage 的存取中斷，您最晚必須在 2025 年 9 月 30 日轉換至 [Adobe Identity](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _IP 限制棄用_：已於 2025 年 7 月 30 日停止支援「[根據 IP 限制 Marketo 登入](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}」的功能。此功能將保持正常運作，直到轉換至 Adobe Identity 的作業完成為止。Adobe Admin Console 中即將推出適用於 Adobe Identity 的全新位置型存取控制功能。

   * _單一登入 (SSO) 棄用_：已於 2025 年 7 月 30 日停止支援 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}。該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。在 Adobe Admin Console 中，Adobe Identity 單一登入必須個別設定。關於設定步驟，請參閱[設定身分識別和單一登入](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

* **棄用「_轉寄給好友_」功能**：自 2025 年 9 月 29 日起，Marketo Engage 2.0 電子郵件 (舊版電子郵件編輯器) 中的「_轉寄給好友_」功能將在所有訂閱中全面棄用。這會影響已經寄出或即將寄出，且使用「轉寄給好友」權杖的電子郵件中的「轉寄給好友」權杖和連結。[了解更多](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **REST API「access_token」參數棄用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將棄用，且於 2026 年 1 月 31 日之後不再提供使用。所有新的和現有的整合都應使用「授權」標頭來驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 棄用**：將於 2026 年 1 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
