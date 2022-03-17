---
description: Sales Insight Actions活動辭彙表 — Marketo文檔 — 產品文檔
title: Sales Insight操作活動辭彙表
hide: true
hidefromtoc: true
source-git-commit: a0cfc190e00ea6f8a9f5ef717566651423638b7d
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Sales Insight操作活動辭彙表 {#sales-insight-actions-activity-glossary}

在Sales Insight Actions中，當賣家：向銷售活動添加銷售線索、向他們發送銷售電子郵件或撥打出站銷售電話，該線索將記錄在Marketo活動歷史記錄下。 此外，當潛在客戶參與電子郵件、開啟、按一下和回復時，它也會被記錄。

以下活動將從Sales Insight Actions記錄到Marketo。

>[!NOTE]
>
>這些活動和屬性可從我們的REST和批量API中使用。

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
  <td>模板ID</td>
 </tr>
 <tr>
  <td>銷售模板URL</td>
 </tr>
 <tr>
  <td>銷售活動URL</td>
 </tr>
 <tr>
  <td>銷售模板名稱</td>
 </tr>
 <tr>
  <td>電子郵件主題</td>
 </tr>
 <tr>
  <td>銷售活動名稱</td>
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
  <td>模板ID</td>
 </tr>
 <tr>
  <td>銷售模板URL</td>
 </tr>
 <tr>
  <td>銷售活動URL</td>
 </tr>
 <tr>
  <td>銷售模板名稱</td>
 </tr>
 <tr>
  <td>電子郵件主題</td>
 </tr>
 <tr>
  <td>銷售活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="10">已按一下銷售電子郵件</th>
  <td>連結</td>
 </tr>
 <tr>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>模板ID</td>
 </tr>
 <tr>
  <td>銷售模板URL</td>
 </tr>
 <tr>
  <td>銷售活動URL</td>
 </tr>
 <tr>
  <td>銷售模板名稱</td>
 </tr>
 <tr>
  <td>電子郵件主題</td>
 </tr>
 <tr>
  <td>銷售活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
<tr>
  <th rowspan="3">已回復銷售電子郵件</th>
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
  <td>銷售呼叫主題</td>
 </tr>
 <tr>
  <td>銷售活動名稱</td>
 </tr>
 <tr>
  <td>銷售活動URL</td>
 </tr>
 <tr>
  <td>已呼叫的銷售電話號碼</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售呼叫持續時間</td>
 </tr>
 <tr>
  <td>銷售呼叫錄制URL</td>
 </tr>
  <tr>
  <td>銷售呼叫應答者</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="6">添加到銷售活動</th>
  <td>銷售活動名稱</td>
 </tr>
 <tr>
  <td>銷售呼叫狀態</td>
 </tr>
 <tr>
  <td>銷售活動URL</td>
 </tr>
 <tr>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售活動ID</td>
 </tr>
 <tr>
  <th rowspan="6">從銷售活動中刪除</th>
  <td>銷售活動名稱</td>
 </tr>
 <tr>
  <td>銷售呼叫狀態</td>
 </tr>
 <tr>
  <td>銷售活動URL</td>
 </tr>
 <tr>
  <td>發送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售活動ID</td>
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
   <td><strong>詳細資訊</strong></td> 
   <td>退回錯誤消息詳細資訊。</td> 
  </tr> 
  <tr> 
   <td><strong>電子郵件</strong></td> 
   <td>已跳轉的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>連結</strong></td> 
   <td>已按一下的URL。</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo銷售人員ID</strong></td> 
   <td>Sales Insight Actions中人員記錄的唯一ID。</td> 
  </tr> 
  <tr> 
   <td><strong>接收者</strong></td> 
   <td>發送電子郵件的人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫應答者</strong></td> 
   <td>應答呼叫的人員的姓名。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫持續時間</strong></td> 
   <td>呼叫長度（秒）。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫由</strong></td> 
   <td>撥打電話的銷售人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫錄制URL</strong></td> 
   <td>呼叫錄制的URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫狀態</strong></td> 
   <td>將保存呼叫的最終呼叫狀態，包括：已完成，無應答，已取消，失敗。</td> 
  </tr>
  <tr> 
   <td><strong>銷售呼叫主題</strong></td> 
   <td>撥號器中銷售用戶選擇的呼叫結果。</td> 
  </tr>
  <tr> 
   <td><strong>銷售活動ID</strong></td> 
   <td>Sales Insight Actions中Sales Campaign資產的唯一ID。</td> 
  </tr>
  <tr> 
   <td><strong>銷售活動名稱</strong></td> 
   <td>銷售活動的名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售活動URL</strong></td> 
   <td>銷售活動的Sales Insight活動URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電子郵件主題</strong></td> 
   <td>電子郵件主題行，後跟唯一ID(例如：我的主題行(SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>已呼叫的銷售電話號碼</strong></td> 
   <td>由Sales調用的電話號碼。</td> 
  </tr>
  <tr> 
   <td><strong>銷售模板名稱</strong></td> 
   <td>Sales Insight Actions中電子郵件模板的名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售模板URL</strong></td> 
   <td>電子郵件模板的Sales Insight Actions URL。</td> 
  </tr>
  <tr> 
   <td><strong>發送者</strong></td>
   <td>發送電子郵件的人員的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td>活動的來源。 將在10月21日發行前設定為Sales Insight Actions活動的「Tout」。 在10月21日發佈後，將是Sales Insight Actions活動的「Sales App」。</td>
  </tr> 
  <tr> 
   <td><strong>模板ID</strong></td> 
   <td>當源為Tout時，模板ID將是MarketoSales Insight Actions模板ID。 使用此選項可以針對特定模板，而不是可能存在於多個模板中的主題行。
</td> 
  </tr> 
 </tbody> 
</table>
