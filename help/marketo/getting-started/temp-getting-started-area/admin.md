---
description: 新區域 — Marketo檔案 — 產品檔案
title: 新區域
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 7d8cdb2da42769ee0326a3d585ad32a3405dfac1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 2%

---

# 新區域：管理員檢查清單 {#new-area-admin-checklist}

介紹文字。

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th>區域 </th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色 </td>
    <td><li>檢閱預先建立的角色，並確認每個角色具有的許可權/存取權。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">建立新角色</a> 或 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">編輯角色</a> 根據您組織的需求以及使用者登入的頻率。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">將使用者指派給適當的角色</a>.</li>
    <li>為使用者指派角色後，可檢視每個角色的使用者數量。</li>  <li>為每個API使用者實作唯一的角色，以方便疑難排解。</li></td>
  </tr>
  <tr>
    <td>文件 </td>
    <td>為您的組織定義使用者和角色。 <br>定義新增使用者/管理員的程式。 </td>
  </tr>
  <tr>
    <td>沙箱（如果適用） </td>
    <td>如果您有沙箱，請檢閱上述類別。 </td>
  </tr>
</tbody>
</table>

## 工作區與分割區 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作區與分割區 </td>
    <td><li>決定數量<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> 工作區</a> 和/或分割您的組織所需的和 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">每個工作區有多少使用者有存取權。</a></li>
    <li>定義每個工作區和分割區的主要用途。</li>
    <li>定義工作區與分割區之間的關係。</li></td>
  </tr>
  <tr>
    <td>文件 </td>
    <td><li>記錄工作區的定義方式以及它與資料庫分割的相關性（亦即，可看到每個人的全域工作區，而不是企業部門）。</li>
    <li>將新記錄匯入適當的資料分割。</li>
    <li>在CRM中定義將使用者放入適當分割的值。</li></td>
  </tr>
</tbody>
</table>

## Smart Campaign設定 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign設定 </td>
    <td><li>新增 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">Smart Campaign大小限制</a>，防止不小心以電子郵件傳送整個資料庫。</li>
    <li>啟用Smart Campaigns的人員限制</li></td>
  </tr>
</tbody>
</table>

## 電子郵件設定 {#email-settings}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>電子郵件預設值</td>
    <td><li>在「品牌化網域」下，選取您的網域並新增您的電子郵件CNAME。 其格式應為： [EmailTrackingCNAME]。[CompanyDomain].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">設定SPF與DKIM</a> 以取得電子郵件傳遞能力。</li></td>
  </tr>
</tbody>
</table>

## 通訊限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通訊限制</td>
    <td><li>地標 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">通訊限制</a>.</li>
    <li>判斷您的企業是否需要通訊限制的原則。</li></td>
  </tr>
</tbody>
</table>

## 標記 {#tags}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>頻道</td>
    <td><li>定義使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">管道</a>.</li></td>
  </tr>
  <tr>
    <td>標記 </td>
    <td><li>定義使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">標籤</a>.</li></td>
  </tr>
  <tr>
    <td>行事曆（如果適用） </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">問題行銷行事曆座位</a> 提供給需要存取許可權的使用者。</li> 
    <li>設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">行事曆</a>.</li></td>
  </tr>
</tbody>
</table>

## 資料庫管理 {#database-management}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>欄位管理</td>
    <td><li>實作命名慣例 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">自訂欄位。</a> 例如，以「MKTO」開頭。</li>
    <li>選擇您同步的欄位。 您同步的欄位越多，同步週期就越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">封鎖欄位更新</a> 您想要寫入一次（即原始潛在客戶來源、原始潛在客戶來源詳細資料、首次接觸UTM欄位等）。</li></td>
  </tr>
  <tr>
    <td>自訂活動 </td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">自訂活動</a> 特定於您的企業。</li></td>
  </tr>
  <tr>
    <td>自訂物件 </td>
    <td><li>檢視數量 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">自訂物件</a> 您需要。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">將這些自訂物件同步至您的CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## 整合 {#integrations}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>起始CRM同步。 請根據貴公司使用的CRM從下列專案中選擇： <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>識別存取CRM所需的存取權型別。</li>
    <li>識別您的CRM管理員以進行疑難排解。</li></td>
  </tr>
  <tr>
    <td>銷售分析（如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">設定Sales Insight。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">將名額發給適當的使用者。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">設定API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">自訂潛在客戶分數。</a></li></td>
  </tr>
</tbody>
</table>
