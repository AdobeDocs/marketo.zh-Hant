---
description: 銷售活動字彙表 — Marketo檔案 — 產品檔案
title: 銷售活動字彙表
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 6%

---

# 銷售活動字彙表 {#sales-activity-glossary}

在Sales Connect中，當賣家：將銷售機會新增至銷售步調、傳送電子郵件給他們，或使通話成為活動時，其將記錄在Marketo活動歷史記錄下。 此外，當銷售機會與電子郵件、開啟、點按和回覆互動時，也會記錄下來。

以下活動將從[!DNL Sales Connect]記錄到Marketo。

>[!NOTE]
>
>這些活動和屬性可從REST和批次API使用。

## 活動 {#activities}

<table>
 <tr>
  <th>銷售活動</th>
  <th>屬性</th>
 </tr>
 <tr>
  <th rowspan="9">傳送銷售電子郵件</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template] 名稱</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="9"> 開啟銷售電子郵件</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="10">已點按的銷售電子郵件</th>
  <td>[!UICONTROL Link]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
<tr>
  <th rowspan="3">已回覆銷售電子郵件</th>
  <td>[!UICONTROL Received By]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">已接聽的銷售電話</th>
  <td>[!UICONTROL Sales Call Made By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Phone Number Called]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Duration]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Recording URL]</td>
 </tr>
  <tr>
  <td>[!UICONTROL Sales Call Answered By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="6">新增至銷售行銷活動</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="6">從銷售行銷活動中移除</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>來源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="5">銷售電子郵件退回</th>
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
  <td>範本 ID</td>
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
   <td><strong>[!UICONTROL Details]</strong></td> 
   <td>退回錯誤訊息詳細資料。</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Email]</strong></td> 
   <td>退回的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Link]</strong></td> 
   <td>被點按的URL。</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Marketo Sales Person ID]</strong></td> 
   <td>[!DNL Sales Connect]中個人記錄的唯一識別碼。</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Received By]</strong></td> 
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Answered By]</strong></td> 
   <td>接聽電話的人員姓名。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Duration]</strong></td> 
   <td>通話的秒數長度。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Made By]</strong></td> 
   <td>撥打電話的銷售人員的電子郵件地址。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Recording URL]</strong></td> 
   <td>通話錄製URL。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Status]</strong></td> 
   <td>將會儲存通話的最終通話狀態，包括：已完成、無接聽、已取消、失敗。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Subject]</strong></td> 
   <td>由撥號器中的銷售使用者選取的通話結果。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign ID]</strong></td> 
   <td>[!DNL Sales Connect]中促銷活動資產的唯一識別碼。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td> 
   <td>促銷活動名稱。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td> 
   <td>[!DNL Sales Connect] 促銷活動URL。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td> 
   <td>電子郵件的主旨行後面跟著唯一識別碼(例如：我的主旨行(MSC-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Phone Number Called]</strong></td> 
   <td>銷售人員呼叫的電話號碼。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Template Name]</strong></td> 
   <td>[!DNL Sales Connect]中電子郵件範本的名稱。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Template URL]</strong></td> 
   <td>[!DNL Sales Connect] 電子郵件範本的URL。</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sent By]</strong></td>
   <td>傳送電子郵件之人員的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Source]</strong></td> 
   <td>活動的Source。 在2021年10月發行前，將針對[!DNL Sales Connect]個活動設為「Tout」。 在2021年10月發行後，將成為[!DNL Sales Connect]活動的「銷售應用程式」。</td>
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Template ID]</strong></td> 
   <td>當來源為Tout時，範本識別碼將是[!DNL Marketo Sales Connect]範本識別碼。 使用此項來鎖定特定範本，而非可能存在於多個範本的主旨列。
</td> 
  </tr> 
 </tbody> 
</table>
