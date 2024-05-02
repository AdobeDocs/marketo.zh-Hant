---
description: 設定新Marketo Engage執行處理的「資料庫」段落。
title: 新執行個體最佳實務 — 資料庫檢查清單
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: 3004885d1b6b986eb30072d2f67c5bd29ad251c7
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 2%

---

# 新執行個體最佳實務：資料庫檢查清單 {#new-instance-best-practices-database-checklist}

您可以在「資料庫」段落中找到執行個體中人員的主要屬性。 進一步瞭解在資料庫中瀏覽不同清單和區段以及管理人員記錄所需的步驟。

記得下載檢查清單 [連結] 並追蹤您的進度。

## 系統智慧清單 {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>所有人員</td>
    <td><li>決定與您的CRM實作1:1同步或套用篩選器以限制從系統到系統的移動人員和時間。</li> 
    <li>檢視您的使用者總人數和行銷人員總數 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank">Marketo Engage資料庫</a>.</li></td>
  </tr>
  <tr>
    <td>封鎖清單</td>
    <td><li>定義封鎖清單條件。 考慮將競爭者的網域新增至 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">封鎖清單</a> 以防止他們收到您的任何電子郵件。</li></td>
  </tr>
  <tr>
    <td>行銷活動已暫停</td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">行銷已暫停</a> 條件。</li></td>
  </tr>
  <tr>
    <td>退回的電子郵件地址 </td>
    <td><li>定義退回電子郵件地址的條件。</li>
    <li>檢閱電子郵件無效類別中的人員，並檢視其電子郵件是否需要 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">手動重設</a>.</li></td>
  </tr>
  <tr>
    <td>可能的重複專案</td>
    <td><li>檢閱可能重複專案清單中的人員。</li> 
    <li>定義您的重複管理策略，以決定您是否要 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">手動合併人員</a>.</li>  
    <li>如果您有CRM整合，請定義流程和帳戶 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">在您的CRM中合併銷售機會的影響</a>.</li></td>
  </tr>
  <tr>
    <td>無贏取計畫</td>
    <td><li>在您的方案範本中建立行銷活動，以設定贏取方案，尤其是使用全域表單時。</li></td>
  </tr>
  <tr>
    <td>已取消訂閱的人員</td>
    <td><li>檢閱您的條件 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank">已取消訂閱的人員</a>.</li></td>
  </tr>
</tbody>
</table>

## 群組智慧清單 {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>群組智慧清單</td>
    <td><li>請注意建立群組智慧列示，這樣就不會有重複的清單。</li>
    <li>追蹤資料庫中的主要清單。</li></td>
  </tr>
</tbody>
</table>

## 區段 {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>區段</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank">建立區段</a> 根據您的業務需求而定。 每個訂閱限製為20個區段，每個區段內最多100個區段。</li></td>
  </tr>
</tbody>
</table>
