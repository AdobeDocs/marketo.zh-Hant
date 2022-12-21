---
description: Sales Insight Actions活動字彙表 — Marketo檔案 — 產品檔案
title: Sales Insight Actions活動辭匯表
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 2%

---

# Sales Insight Actions活動辭匯表 {#sales-insight-actions-activity-glossary}

在Sales Insight Actions中，當賣家：新增銷售機會至銷售促銷活動、傳送銷售電子郵件或進行外站銷售呼叫，該銷售機會將記錄在該銷售機會的Marketo活動記錄下。 此外，當銷售機會與電子郵件、開啟、點按和回覆互動時，也會記錄該銷售機會。

下列活動將從Sales Insight Actions記錄至Marketo。

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
   <td>「銷售分析動作」中人員記錄的唯一ID。</td> 
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
   <td>Sales Insight Actions中Sales Campaign資產的唯一ID。</td> 
  </tr>
  <tr> 
   <td><strong>銷售促銷活動名稱</strong></td> 
   <td>銷售促銷活動的名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售促銷活動URL</strong></td> 
   <td>銷售促銷活動的銷售分析操作URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電子郵件主題</strong></td> 
   <td>電子郵件的主旨行，後面接著唯一ID(例如：我的主題行(SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>已呼叫銷售電話號碼</strong></td> 
   <td>由銷售部呼叫的電話號碼。</td> 
  </tr>
  <tr> 
   <td><strong>銷售模板名稱</strong></td> 
   <td>Sales Insight Actions中的電子郵件模板名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售模板URL</strong></td> 
   <td>電子郵件範本的Sales Insight Actions URL。</td> 
  </tr>
  <tr> 
   <td><strong>發送者</strong></td>
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td>活動來源。 在』21年10月發行之前，將會設為「銷售分析動作」活動的「輸出」。 在』21年10月發行後，將是「銷售分析動作」活動的「銷售應用程式」。</td>
  </tr> 
  <tr> 
   <td><strong>範本ID</strong></td> 
   <td>當來源輸出時，範本ID將會是Marketo Sales Insight Actions範本ID。 使用此功能可鎖定特定範本，而非多個範本中可能存在的主旨行。
</td> 
  </tr> 
 </tbody> 
</table>
