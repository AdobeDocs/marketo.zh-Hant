---
description: 設定新Marketo Engage執行處理的「資料庫」段落。
title: 新增區域資料庫
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 1966bc6f-9384-4c51-b3aa-57d5e52781f1
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# 新區域：資料庫檢查清單 {#new-area-database-checklist}

瞭解如何在新的Marketo Engage執行個體中為「資料庫」區段實作必要的步驟。 遵循「實作新執行個體」指南，並追蹤進行中的工作，協助您設定執行個體，以提高長期效率。

## 系統智慧清單 {#system-smart-lists}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>所有人員</td>
    <td><li>決定要與CRM實作1:1同步或套用篩選器，以限制從系統到系統的移動者及移動時間。</li> 
    <li>檢視您的使用者總人數和行銷人員總數 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank" rel="noopener noreferrer">資料庫</a>.</li></td>
  </tr>
  <tr>
    <td>封鎖清單</td>
    <td><li>定義封鎖清單條件。 考慮將競爭者的網域新增至 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank" rel="noopener noreferrer">封鎖清單</a> 以防止他們收到任何行銷和營運電子郵件。</li></td>
  </tr>
  <tr>
    <td>行銷活動已暫停</td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank" rel="noopener noreferrer">行銷已暫停</a> 條件。</li></td>
  </tr>
  <tr>
    <td>退回的電子郵件地址 </td>
    <td><li>定義退回電子郵件地址的條件。</li>
    <li>檢閱電子郵件無效類別中的人員，並檢視其電子郵件是否需要 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank" rel="noopener noreferrer">手動重設</a>.</li></td>
  </tr>
  <tr>
    <td>可能的重複專案</td>
    <td><li>檢閱可能重複專案清單中的人員。</li> 
    <li>定義您的重複管理策略以確定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank" rel="noopener noreferrer">手動合併人員</a> 也可能不會。</li>  
    <li>如果您有CRM整合，您應該定義流程和帳戶 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank" rel="noopener noreferrer">CRM中合併銷售機會的影響</a>.</li></td>
  </tr>
  <tr>
    <td>無贏取計畫</td>
    <td><li>在您的方案範本中建立行銷活動，以設定贏取方案，尤其是使用全域表單時。</li></td>
  </tr>
  <tr>
    <td>已取消訂閱的人員</td>
    <td><li>檢閱您的條件 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank" rel="noopener noreferrer">已取消訂閱的人員</a>.</li></td>
  </tr>
</tbody>
</table>

## 群組智慧清單 {#group-smart-lists}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>群組智慧清單</td>
    <td><li>請注意建立群組智慧列示，這樣就不會有重複的清單。</li>
    <li>在資料庫中追蹤主要清單。</li></td>
  </tr>
</tbody>
</table>

## 區段 {#segmentation}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>區段</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank" rel="noopener noreferrer">建立區段</a> 根據您的業務需求而定。 每個訂閱限製為20個區段，每個區段內最多100個區段。</li></td>
  </tr>
</tbody>
</table>
