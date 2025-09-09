---
description: 發行說明 — 2025年8月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2025 年 8 月
feature: Release Information
hide: true
hidefromtoc: true
source-git-commit: 07b2e888c31c6e98a3207fad5d277261f7f193af
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 98%

---

# 發行說明：2025 年 8 月 {#release-notes-aug-25}

以下為 2025 年 8 月發行版本中包含的所有功能。請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

以下功能屬於標準發行週期，將於 **2025 年 8 月 22 日**&#x200B;開始發行，其餘功能則會在接下來數週內分階段推出。發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">文件</th>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 報告</strong>：電子郵件績效和電子郵件連結績效報告現在會顯示使用新的電子郵件設計工具建立的電子郵件資料。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 自動完成移除</strong>：權杖個人化編輯器中的「自動完成」選項先前指向了錯誤的物件，已遭移除。目前沒有重新實作此功能的計劃。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 電子郵件預覽最佳化</strong>：部分使用者嘗試在電子郵件/電子郵件範本/片段詳細資料頁面中預覽電子郵件時，遇到載入時間較慢的問題。此體驗已完成最佳化，載入時間可加速 60%。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 範本修正</strong>：部分現成可用的範本出現轉譯問題 (例如在特定瀏覽器/深色模式下無法正確轉譯、影像未對齊、CTA 按鈕錯置及其他問題)。此版本已修正以上所有問題。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>電子郵件設計工具 - 內容鎖定修正</strong>：過去，如果使用內容鎖定建立電子郵件範本，且將此範本用於建立電子郵件，則即使重設電子郵件或選取「變更設計」，內容鎖定仍會存在。此版本已修正此問題。</td>
   <td>已發布</td>
   <td>不適用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>編輯智慧行銷活動限制的權限</strong>：管理員現在可以規定，只有具備權限的使用者才能修改智慧行銷活動的限制。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo Engage Identity 終止服務**：2025 年 8 月，Adobe 已開始逐步停止對於 Marketo Engage Identity (透過 `login.marketo.com` 登入) 的支援。為避免 Marketo Engage 的存取中斷，您最晚必須在 2025 年 9 月 30 日轉換至 [Adobe Identity](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _IP 限制棄用_：已於 2025 年 7 月 30 日停止支援「[根據 IP 限制 Marketo 登入](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}」的功能。此功能將保持正常運作，直到轉換至 Adobe Identity 的作業完成為止。Adobe Admin Console 中即將推出適用於 Adobe Identity 的全新位置型存取控制功能。

   * _單一登入 (SSO) 棄用_：已於 2025 年 7 月 30 日停止支援 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}。該功能將保持正常運作，直到轉換至 Adobe Identity 的過程完成為止。在 Adobe Admin Console 中，Adobe Identity 單一登入必須個別設定。關於設定步驟，請參閱[設定身分識別和單一登入](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html){target="_blank"}。

* **棄用「_轉寄給好友_」功能**：自 2025 年 9 月 29 日起，Marketo Engage 2.0 電子郵件 (舊版電子郵件編輯器) 中的「_轉寄給好友_」功能將在所有訂閱中全面棄用。這會影響已經寄出或即將寄出，且使用「轉寄給好友」權杖的電子郵件中的「轉寄給好友」權杖和連結。[了解更多](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **REST API「存取權杖」參數棄用**：用於驗證 Marketo REST API 呼叫的 `access_token` 查詢參數將停止適用，且於 2025 年 10 月 31 日之後不再提供使用。所有新的和現有的整合都應使用「授權」標頭驗證 REST API 呼叫，方法[如此處所述](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 棄用**：將於 2025 年 10 月 31 日停止支援 Marketo SOAP API。使用 SOAP API 功能的服務應移轉至 [REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
