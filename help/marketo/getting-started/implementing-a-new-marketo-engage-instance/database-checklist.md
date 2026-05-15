---
description: 為您新的Marketo Engage執行個體設定「資料庫」區段。
title: 新執行個體最佳實務 — 資料庫檢查清單
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
TQID: https://experienceleague.adobe.com/yHZP1MXkAnmnz3zeucu2Bdm6FrCVtmnX9opKWiIJTAA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 451
ht-degree: 5%

---

# 新執行個體最佳做法：資料庫檢查清單 {#new-instance-best-practices-database-checklist}

您可以在「資料庫」段落中找到執行個體中人員的主要屬性。 進一步瞭解在資料庫中瀏覽不同清單和區段以及管理人員記錄所需的步驟。

記得要[下載檢查清單](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)並追蹤您的進度。

## 系統智慧清單 {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>所有人員</td>
    <td><li>決定與您的CRM實作1:1同步或套用篩選器以限制從系統到系統的移動人員和時間。</li>
    <li>檢閱<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=zh-Hant" target="_blank">Marketo Engage資料庫</a>中的總人數和行銷人員。</li></td>
  </tr>
  <tr>
    <td>封鎖清單</td>
    <td><li>定義封鎖清單條件。 請考慮將競爭者的網域新增至您的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=zh-Hant" target="_blank">封鎖清單</a>，以防止他們收到您的任何電子郵件。</li></td>
  </tr>
  <tr>
    <td>行銷活動暫停</td>
    <td><li>定義<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">行銷活動已暫停</a>條件。</li></td>
  </tr>
  <tr>
    <td>退回的電子郵件地址 </td>
    <td><li>定義退回電子郵件地址的條件。</li>
    <li>檢閱「電子郵件無效」類別中的人員，並判斷其電子郵件是否需要<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=zh-Hant" target="_blank">手動重設</a>。</li></td>
  </tr>
  <tr>
    <td>可能的複製</td>
    <td><li>檢閱可能重複專案清單中的人員。</li>
    <li>定義您的重複管理策略，以決定是否要手動<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=zh-Hant" target="_blank">合併人員</a>。</li>
    <li>如果您有CRM整合，請針對在CRM</a>中合併潛在客戶的<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">效果定義程式與帳戶。</li></td>
  </tr>
  <tr>
    <td>無贏取方案</td>
    <td><li>在您的方案範本中建立行銷活動，以設定贏取方案，尤其是使用全域表單時。</li></td>
  </tr>
  <tr>
    <td>取消訂閱的人員</td>
    <td><li>檢閱您的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=zh-Hant" target="_blank">已取消訂閱的使用者</a>條件。</li></td>
  </tr>
</tbody>
</table>

## 群組智慧清單 {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
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

## 細分 {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">區域圖</th>
    <th style="width:79%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>細分</td>
    <td><li>根據您的業務需求<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=zh-Hant" target="_blank">建立區段</a>。 每個訂閱限製為20個區段，每個區段內最多100個區段。</li></td>
  </tr>
</tbody>
</table>
