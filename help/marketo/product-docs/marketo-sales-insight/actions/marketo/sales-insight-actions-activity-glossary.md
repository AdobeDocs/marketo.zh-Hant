---
description: 銷售分析動作活動字彙表 — Marketo檔案 — 產品檔案
title: 銷售分析動作活動字彙表
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
source-git-commit: 3e0836fd9f40436564c7b2d8bb58a7f771e49c33
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 2%

---

# 銷售分析動作活動字彙表 {#sales-insight-actions-activity-glossary}

在「銷售分析動作」中，當賣家：將銷售線索新增至銷售促銷活動、傳送銷售電子郵件或進行對外銷售通話時，會記錄在該銷售線索的Marketo活動歷史記錄下。 此外，當銷售機會與電子郵件、開啟、點按和回覆互動時，也會記錄下來。

以下活動將會從Sales Insight Actions記錄到Marketo。

>[!NOTE]
>
>這些活動和屬性可從我們的REST和批次API使用。

## 活動 {#activities}

<table>
 <tr>
  <th>銷售活動</th>
  <th>屬性</th>
 </tr>
 <tr>
  <th rowspan="9">傳送銷售電子郵件</th>
  <td>傳送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>範本ID</td>
 </tr>
 <tr>
  <td>銷售範本URL</td>
 </tr>
 <tr>
  <td>促銷活動URL</td>
 </tr>
 <tr>
  <td>銷售範本名稱</td>
 </tr>
 <tr>
  <td>電子郵件主旨</td>
 </tr>
 <tr>
  <td>促銷活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="9">開啟銷售電子郵件</th>
  <td>傳送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>範本ID</td>
 </tr>
 <tr>
  <td>銷售範本URL</td>
 </tr>
 <tr>
  <td>促銷活動URL</td>
 </tr>
 <tr>
  <td>銷售範本名稱</td>
 </tr>
 <tr>
  <td>電子郵件主旨</td>
 </tr>
 <tr>
  <td>促銷活動名稱</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="10">已點按的銷售電子郵件</th>
  <td>連結</td>
 </tr>
 <tr>
  <td>傳送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>範本ID</td>
 </tr>
 <tr>
  <td>銷售範本URL</td>
 </tr>
 <tr>
  <td>促銷活動URL</td>
 </tr>
 <tr>
  <td>銷售範本名稱</td>
 </tr>
 <tr>
  <td>電子郵件主旨</td>
 </tr>
 <tr>
  <td>促銷活動名稱</td>
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
  <th rowspan="11">已接聽的銷售電話</th>
  <td>進行銷售通話者</td>
 </tr>
 <tr>
  <td>銷售電話狀態</td>
 </tr>
 <tr>
  <td>銷售電話主題</td>
 </tr>
 <tr>
  <td>促銷活動名稱</td>
 </tr>
 <tr>
  <td>促銷活動URL</td>
 </tr>
 <tr>
  <td>已呼叫的銷售電話號碼</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>銷售電話期間</td>
 </tr>
 <tr>
  <td>銷售電話錄音URL</td>
 </tr>
  <tr>
  <td>銷售電話接聽者</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <th rowspan="6">新增至銷售行銷活動</th>
  <td>促銷活動名稱</td>
 </tr>
 <tr>
  <td>銷售電話狀態</td>
 </tr>
 <tr>
  <td>促銷活動URL</td>
 </tr>
 <tr>
  <td>傳送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>促銷活動ID</td>
 </tr>
 <tr>
  <th rowspan="6">從銷售行銷活動中移除</th>
  <td>促銷活動名稱</td>
 </tr>
 <tr>
  <td>銷售電話狀態</td>
 </tr>
 <tr>
  <td>促銷活動URL</td>
 </tr>
 <tr>
  <td>傳送者</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>促銷活動ID</td>
 </tr>
 <tr>
  <th rowspan="5">銷售電子郵件跳出</th>
  <td>詳細資料</td>
 </tr>
 <tr>
  <td>電子郵件</td>
 </tr>
 <tr>
  <td>傳送者</td>
 </tr>
 <tr>
  <td>Marketo銷售人員ID</td>
 </tr>
 <tr>
  <td>範本ID</td>
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
   <td>退回錯誤訊息詳細資料。</td> 
  </tr> 
  <tr> 
   <td><strong>電子郵件</strong></td> 
   <td>退回的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>連結</strong></td> 
   <td>已點按的URL。</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo銷售人員ID</strong></td> 
   <td>銷售分析動作中個人記錄的唯一ID。</td> 
  </tr> 
  <tr> 
   <td><strong>接收者</strong></td> 
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電話接聽者</strong></td> 
   <td>接聽電話的人員姓名。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電話期間</strong></td> 
   <td>呼叫的秒數長度。</td> 
  </tr>
  <tr> 
   <td><strong>進行銷售通話者</strong></td> 
   <td>撥打電話的銷售人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電話錄音URL</strong></td> 
   <td>通話錄製的URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電話狀態</strong></td> 
   <td>將會儲存呼叫的最終呼叫狀態，包括：已完成、無應答、已取消、失敗。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電話主題</strong></td> 
   <td>撥號器中的銷售使用者所選取的通話結果。</td> 
  </tr>
  <tr> 
   <td><strong>促銷活動ID</strong></td> 
   <td>銷售分析動作中促銷活動資產的唯一ID。</td> 
  </tr>
  <tr> 
   <td><strong>促銷活動名稱</strong></td> 
   <td>促銷活動名稱。</td> 
  </tr>
  <tr> 
   <td><strong>促銷活動URL</strong></td> 
   <td>銷售促銷活動的銷售分析動作URL。</td> 
  </tr>
  <tr> 
   <td><strong>銷售電子郵件主旨</strong></td> 
   <td>電子郵件主旨行後面跟著唯一ID (例如：我的主旨行(SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>已呼叫的銷售電話號碼</strong></td> 
   <td>銷售人員呼叫的電話號碼。</td> 
  </tr>
  <tr> 
   <td><strong>銷售範本名稱</strong></td> 
   <td>Sales Insight動作中的電子郵件範本名稱。</td> 
  </tr>
  <tr> 
   <td><strong>銷售範本URL</strong></td> 
   <td>電子郵件範本的銷售分析動作URL。</td> 
  </tr>
  <tr> 
   <td><strong>傳送者</strong></td>
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>來源</strong></td> 
   <td>活動的來源。 針對2021年10月發行版本之前的銷售分析動作活動，將會設定為「Tout」。 在2021年10月發行版本之後，將會成為銷售分析動作活動的「銷售應用程式」。</td>
  </tr> 
  <tr> 
   <td><strong>範本ID</strong></td> 
   <td>當來源為Tout時，範本ID將為Marketo Sales Insight動作範本ID。 使用此項來鎖定特定範本，而非可能存在於多個範本中的主旨行。
</td> 
  </tr> 
 </tbody> 
</table>
