---
description: 發行說明 — 2024年4月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2024 年 4 月
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 21%

---

# 發行說明：2024 年 4 月 {#release-notes-apr-24}

下方提供2024年4月發行版本包含的所有功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

如需 Adobe Dynamic Chat 特定的發行說明，[請參閱這裡](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於&#x200B;**2024年4月26日**&#x200B;開始發行，在接下來的幾週內分階段推出剩餘功能。 發行的功能和日期可能有所變更。如需了解各項功能的狀態，請查看其旁邊欄位。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
     <tr>
   <td><strong>互動式網路研討會增強功能</strong>：您現在可以讓主機和主持人新增網路研討會標題、重新命名聊天室，以及在事件傳送後手動同步互動資料。</td>
   <td>已發布</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">建立互動式網路研討會</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">手動同步</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>稽核軌跡增強功能</strong>：
   現在可以在「稽核軌跡」中擷取新型別的動作，以取得「欄位管理」中所做的變更、使用者與角色的變更，以及從清單與智慧列示匯出的人員計數。</td>
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>新使用者和角色許可權</strong>：新許可權已推出，讓使用者能更精細地存取Marketo Engage。 控制先前未啟用的管理員部分（例如新體驗和預測對象）、分割許可權以分別授予資產稽核軌跡和管理稽核軌跡的存取權，以及使用新的資產和資料夾的建立和移動許可權來防止唯讀使用者進行變更。
   <p>雖然新許可權將於4月26日起顯示在您的Marketo Engage執行個體中，但目前仍為被動許可權，將於本季度晚些時候可供存取。
   <li>存取Adobe Experience Manager</li>
   <li>存取Adobe組織對應</li>
   <li>存取管理員稽核軌跡</li>
   <li>存取資產稽核軌跡</li>
   <li>存取新體驗</li>
   <li>存取預測對象</li>
   <li>建立報告</li>
   <li>建立清單</li>
   <li>匯出行銷活動內容</li>
   </td>
   <td>已發布</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">角色權限說明</a></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **活動API更新**： 4月26日，我們將新增數個屬性至網頁型與電子郵件型活動，這些活動會在您使用[Marketo REST API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}擷取活動時傳回。 下列活動現在包含「瀏覽器」、「平台」、「裝置」和「使用者代理程式」屬性。 呼叫[Get Activity Types](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"}端點以檢閱每個活動的屬性詳細資料。

**網頁型活動**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">活動</th>
   <th style="width:70%">新新增的屬性</th>
   </tr>
  <tr>
   <td>造訪網頁</td>
   <td>瀏覽器、平台、裝置</td>
  </tr>
   <tr>
   <td>填寫表單</td>
   <td>瀏覽器、平台、裝置</td>
  </tr>
  <tr>
   <td>按一下連結</td>
   <td>瀏覽器、平台、裝置</td>
  </tr>
 </tbody>
</table>

**電子郵件活動**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">活動</th>
   <th style="width:70%">新新增的屬性</th>
  </tr>
   <tr>
   <td>傳送電子郵件</td>
   <td>瀏覽器、平台、裝置、使用者代理程式</td>
  </tr>
   </tr>
  <tr>
   <td>電子郵件已傳遞</td>
   <td>瀏覽器、平台、裝置、使用者代理程式</td>
  </tr>
   <tr>
   <td>電子郵件已退回</td>
   <td>瀏覽器、平台、裝置、使用者代理程式</td>
  </tr>
  <tr>
   <td>取消訂閱電子郵件</td>
   <td>瀏覽器、平台、裝置</td>
  </tr>
  <tr>
   <td>開啟電子郵件</td>
   <td>瀏覽器</td>
  </tr>
   <tr>
   <td>點按電子郵件</td>
   <td>瀏覽器</td>
  </tr>
  <tr>
   <td>電子郵件已軟退回</td>
   <td>瀏覽器、平台、裝置、使用者代理程式</td>
  </tr>
 </tbody>
</table>
