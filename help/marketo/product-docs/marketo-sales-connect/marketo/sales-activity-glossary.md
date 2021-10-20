---
description: 銷售活動字彙表 — Marketo檔案 — 產品檔案
title: 銷售活動辭匯表
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 42ddb44100a041a09ff4a68c02ccf6aabb2d953e
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 1%

---

# 銷售活動辭匯表 {#sales-activity-glossary}

在Sales Connect中，當賣家：新增銷售機會至銷售順序、傳送電子郵件或呼叫活動，則會記錄在Marketo活動記錄下。 此外，當銷售機會與電子郵件互動時，系統也會記錄開啟、點按和回覆。

以下活動將從Sales Connect記錄到Marketo。

>[!NOTE]
>
>這些活動和屬性可供我們的REST和大量API使用。

## 活動 {#activities}

<table>
 <tr>
  <th>銷售活動</th>
  <th>屬性</th>
 </tr>
 <tr>
  <th rowspan="9">發送銷售電子郵件</th>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>範本ID</td>
 </tr>
 <tr>
  <td>銷售模板URL</td>
 </tr>
 <tr>
  <td>銷售促銷活動URL</td>
 </tr>
 <tr>
  <td>銷售模板名稱</td>
 </tr>
 <tr>
  <td>電子郵件主旨</td>
 </tr>
 <tr>
  <td>銷售促銷活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="9">開啟銷售電子郵件</th>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>範本ID</td>
 </tr>
 <tr>
  <td>銷售模板URL</td>
 </tr>
 <tr>
  <td>銷售促銷活動URL</td>
 </tr>
 <tr>
  <td>銷售模板名稱</td>
 </tr>
 <tr>
  <td>電子郵件主旨</td>
 </tr>
 <tr>
  <td>銷售促銷活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="10">已點擊銷售電子郵件</th>
  <td>連結</td>
 </tr>
 <tr>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>範本ID</td>
 </tr>
 <tr>
  <td>銷售模板URL</td>
 </tr>
 <tr>
  <td>銷售促銷活動URL</td>
 </tr>
 <tr>
  <td>銷售模板名稱</td>
 </tr>
 <tr>
  <td>電子郵件主旨</td>
 </tr>
 <tr>
  <td>銷售促銷活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
<tr>
  <th rowspan="3">已回覆銷售電子郵件</th>
  <td>接收者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="11">已接收銷售呼叫</th>
  <td>銷售呼叫由</td>
 </tr>
 <tr>
  <td>銷售呼叫狀態</td>
 </tr>
 <tr>
  <td>銷售呼叫主體</td>
 </tr>
 <tr>
  <td>銷售促銷活動名稱</td>
 </tr>
 <tr>
  <td>銷售促銷活動URL</td>
 </tr>
 <tr>
  <td>已呼叫銷售電話號碼</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售呼叫持續時間</td>
 </tr>
 <tr>
  <td>銷售呼叫記錄URL</td>
 </tr>
  <tr>
  <td>應答銷售電話的人</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="6">添加到銷售活動</th>
  <td>銷售促銷活動名稱</td>
 </tr>
 <tr>
  <td>銷售呼叫狀態</td>
 </tr>
 <tr>
  <td>銷售促銷活動URL</td>
 </tr>
 <tr>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售促銷活動ID</td>
 </tr>
 <tr>
  <th rowspan="6">從Sales Campaign中刪除</th>
  <td>銷售促銷活動名稱</td>
 </tr>
 <tr>
  <td>銷售呼叫狀態</td>
 </tr>
 <tr>
  <td>銷售促銷活動URL</td>
 </tr>
 <tr>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售促銷活動ID</td>
 </tr>
</table>

## 說明 {#descriptions}

<table> 
 <tr>
  <th>屬性</th>
  <th>說明</th>
 </tr>
 <tbody> 
 <tr> 
   <td><strong>詳細資料</strong></td> 
   <td>退信錯誤消息詳細資訊。</td> 
  </tr> 
  <tr> 
   <td><strong>電子郵件</strong></td> 
   <td>跳出的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>連結</strong></td> 
   <td>已點按的URL。</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo銷售人員ID</strong></td> 
   <td>Sales Connect中人員記錄的唯一ID。</td> 
  </tr> 
  <tr> 
   <td><strong>接收者</strong></td> 
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>應答銷售電話的人</strong></td> 
   <td>接聽電話的人員姓名。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫持續時間</strong></td> 
   <td>呼叫長度（以秒為單位）。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫由</strong></td> 
   <td>進行呼叫的銷售人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫記錄URL</strong></td> 
   <td>呼叫記錄的URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫狀態</strong></td> 
   <td>將儲存呼叫的最終呼叫狀態，其中包括：已完成，無應答，已取消，失敗。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫主體</strong></td> 
   <td>呼叫撥號器中銷售用戶選擇的結果。</td> 
  </tr>
  <tr> 
   <td><strong>銷售促銷活動ID</strong></td> 
   <td>Sales Connect中Sales Campaign資產的唯一ID。</td> 
  </tr>
  <tr> 
   <td><strong>銷售促銷活動名稱</strong></td> 
   <td>銷售促銷活動的名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售促銷活動URL</strong></td> 
   <td>銷售活動的銷售連接URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電子郵件主題</strong></td> 
   <td>電子郵件的主旨行。</td> 
  </tr>
  <tr> 
   <td><strong>已呼叫銷售電話號碼</strong></td> 
   <td>由銷售部呼叫的電話號碼。</td> 
  </tr>
  <tr> 
   <td><strong>銷售模板名稱</strong></td> 
   <td>Sales Connect中的電子郵件模板名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售模板URL</strong></td> 
   <td>電子郵件模板的Sales Connect URL。</td> 
  </tr>
  <tr> 
   <td><strong>發送者</strong></td>
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td>活動來源。 將設定為「Tout」（銷售連接）活動。</td> 
  </tr> 
  <tr> 
   <td><strong>範本ID</strong></td> 
   <td>當源為Tout時，模板ID將是Marketo Sales Connect模板ID。 使用此功能可鎖定特定範本，而非多個範本中可能存在的主旨行。
</td> 
  </tr> 
 </tbody> 
</table>
