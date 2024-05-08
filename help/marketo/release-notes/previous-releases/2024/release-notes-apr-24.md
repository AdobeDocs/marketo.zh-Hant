---
description: 發行說明 — 2024年4月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2024年4月
feature: Release Information
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 發行說明： 2024年4月 {#release-notes-apr-24}

下方提供2024年4月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

Adobe Dynamic Chat專屬發行說明 [可在此處找到](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>以星號(![星形](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

## 標準發行週期功能 {#standard-release-cycle-features}

下列功能屬於標準發行週期，並將於以下日期開始發行 **2024年4月26日**，在接下來的幾週內分階段推出剩餘的功能。 發行功能和日期可能會有所變更。 請檢查每個功能旁的狀態。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">狀態</th>
   <th style="width:25%">檔案</th>
  </tr>
     <tr> 
   <td><strong>互動式網路研討會增強功能</strong>：您現在可以讓主機和主持人新增網路研討會標題、重新命名聊天室，以及在事件傳送後手動同步參與資料。</td> 
   <td>已送出</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">建立互動式網路研討會</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">手動同步</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>稽核軌跡增強功能</strong>：現在可以在稽核軌跡中擷取新型別的動作，包括在「欄位管理」中所做的變更、對使用者和角色所做的變更，以及從清單和智慧清單匯出的人員計數。</td> 
   <td><i>即將推出</i></td>
   <td><i>即將推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>新使用者和角色許可權</strong>：新許可權可供使用，為使用者提供更精細的Marketo Engage存取許可權。 控制先前未啟用的管理員部分（例如新體驗和預測對象）、分割許可權以分別授予資產稽核軌跡和管理稽核軌跡的存取權，以及使用新的資產和資料夾的建立和移動許可權來防止唯讀使用者進行變更。 
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
   <td>已送出</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">角色許可權說明</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **活動API更新**：4月26日起，我們將針對當您使用擷取活動時傳回的Web型活動和電子郵件型活動，新增數個屬性 [MARKETO REST API](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} 端點可檢閱每個活動的屬性詳細資料。

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

**電子郵件型活動**

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
   <td>按一下電子郵件</td> 
   <td>瀏覽器</td>
  </tr>
  <tr> 
   <td>電子郵件已軟退回</td> 
   <td>瀏覽器、平台、裝置、使用者代理程式</td>
  </tr>
 </tbody> 
</table>
