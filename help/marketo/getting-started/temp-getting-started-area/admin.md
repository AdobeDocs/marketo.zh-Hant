---
description: 新區域 — Marketo檔案 — 產品檔案
title: 新區域
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 2%

---

# 新區域：管理員檢查清單 {#new-area-admin-checklist}

介紹文字。

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色</td>
    <td><li>檢閱預先建立的角色，並確認每個角色具有的許可權/存取權。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">建立新角色</a> 或 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">編輯角色</a> 根據您組織的需求以及使用者登入的頻率。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">將使用者指派給適當的角色</a>.</li>
    <li>為使用者指派角色後，可檢視每個角色的使用者數量。</li>  <li>為每個API使用者實作唯一的角色，以方便疑難排解。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>文件</td>
    <td>為您的組織定義使用者和角色。 <br>定義新增使用者/管理員的程式。</td>
    <td></td>
  </tr>
  <tr>
    <td>沙箱（如果適用）</td>
    <td>如果您有沙箱，請檢閱上述類別。</td>
    <td></td>
  </tr>
</tbody>
</table>

## 工作區與分割區 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作區與分割區 </td>
    <td><li>決定數量<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> 工作區</a> 和/或分割您的組織所需的和 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">每個工作區有多少使用者有存取權。</a></li>
    <li>定義每個工作區和分割區的主要用途。</li>
    <li>定義工作區與分割區之間的關係。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>文件</td>
    <td><li>記錄工作區的定義方式以及它與資料庫分割的相關性（亦即，可看到每個人的全域工作區，而不是企業部門）。</li>
    <li>將新記錄匯入適當的資料分割。</li>
    <li>在CRM中定義將使用者放入適當分割的值。</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Smart Campaign設定 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign設定 </td>
    <td><li>新增 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">Smart Campaign大小限制</a>，防止不小心以電子郵件傳送整個資料庫。</li>
    <li>啟用Smart Campaigns的人員限制</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 電子郵件設定 {#email-settings}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>電子郵件預設值</td>
    <td><li>在「品牌化網域」下，選取您的網域並新增您的電子郵件CNAME。 其格式應為： [EmailTrackingCNAME]。[CompanyDomain].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">設定SPF與DKIM</a> 以取得電子郵件傳遞能力。</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 通訊限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通訊限制</td>
    <td><li>地標 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">通訊限制</a>.</li>
    <li>判斷您的企業是否需要通訊限制的原則。</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 標記 {#tags}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>頻道</td>
    <td><li>定義使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">管道</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>標記 </td>
    <td><li>定義使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">標籤</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>行事曆（如果適用） </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">問題行銷行事曆座位</a> 提供給需要存取許可權的使用者。</li> 
    <li>設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">行事曆</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 資料庫管理 {#database-management}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>欄位管理</td>
    <td><li>實作命名慣例 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">自訂欄位。</a> 例如，以「MKTO」開頭。</li>
    <li>選擇您同步的欄位。 您同步的欄位越多，同步週期就越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">封鎖欄位更新</a> 您想要寫入一次（即原始潛在客戶來源、原始潛在客戶來源詳細資料、首次接觸UTM欄位等）。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>自訂活動 </td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">自訂活動</a> 特定於您的企業。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>自訂物件 </td>
    <td><li>檢視數量 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">自訂物件</a> 您需要。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">將這些自訂物件同步至您的CRM</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## 整合 {#integrations}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>起始CRM同步。 請根據貴公司使用的CRM從下列專案中選擇： <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>識別存取CRM所需的存取權型別。</li>
    <li>識別您的CRM管理員以進行疑難排解。</li></td>
    <td></td>
  </tr>
  <tr>
    <td>銷售分析（如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">設定Sales Insight。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">將名額發給適當的使用者。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">設定API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">自訂潛在客戶分數。</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>登陸頁面 </td>
    <td>注意：您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您啟動電話時，為您提供IT設定指示檔案。 <br>使用設定您的登入頁面網域 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> 和 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">輸入網域和頁面資訊</a>. 其格式應為： [LandingPageCNAME]。[CompanyDomain].com <br>為您的登入頁面選擇一個CNAME。 部分範例： <br>* **go**。[CompanyDomain].com <br>* **www2**。[CompanyDomain].com <br>* **lp**。[CompanyDomain].com <br>秘訣：簡明扼要！ 較短的URL更容易記憶。 我們建議使用「前往」作為網域。 <br>將Analytics追蹤程式碼(例如Google Analytics或Adobe Analytics)新增至您的登入頁面範本。 </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">編輯登陸頁面設定</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">注意：如果您是Launch Pack客戶，請略過此步驟。 您的顧問會在IT設定指示檔案中為您提供Munchkin程式碼指示。 <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">新增Munchkin追蹤程式碼</a> 至您的網站。 Munchkin程式碼可以是 <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">硬式編碼</a> 或透過Google Tag Manager部署。</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">將Munchkin追蹤程式碼新增至您的網站</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">銷售機會追蹤</a> </td>
  </tr>
  <tr>
    <td>網站服務 </td>
    <td>啟用 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">IP限制</a> 若適用。 <br>決定可以製作的使用者/應用程式 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">API呼叫</a> 在您的例項中。 <br>檢閱將進行API呼叫的所有應用程式，並判斷API呼叫是否需要增加或減少。</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">建立IP型API存取的允許清單 </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（如果適用） </td>
    <td>使用 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>，這是Marketo Engage的原生對話參與管道，您將依照以下步驟繼續使用者許可權設定： <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>確認您的Adobe組織系統管理員是否已授予您Adobe產品管理員角色。 連絡人 <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe客戶服務</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> 以找出貴組織中哪些人擁有主控台中的管理員許可權。 <br>Accept <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">「Dynamic Chat產品管理員」邀請</a>. 此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">歡迎電子郵件</a> 會在您的Marketo Engage執行個體中啟用Dynamic Chat且您被指定為系統管理員時傳送。  <br>將所有適當的使用者指派給Adobe Admin Console中的Marketo Engage產品設定檔。 <br>將使用者新增至產品設定檔之前，您無法在Marketo Engage/管理員/使用者與角色中指派使用者角色。  <br>如果將不需要的使用者新增到多個產品設定檔，您必須從所有產品設定檔中刪除該使用者。 否則，他們仍可存取Dynamic Chat。 </td>
    <td> </td>
  </tr>
  <tr>
    <td>啟動點（如果適用） </td>
    <td>設定任何必要的專案 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">啟動點</a> 為貴企業提供的服務。  <br>注意：互動式網路研討會是內建的網路研討會功能，與Adobe Connect原生整合。 不需要額外的整合，但您的執行個體將需要 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">同步至Adobe Connect as a LaunchPoint Service。</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">其他整合</a> </td>
  </tr>
  <tr>
    <td>Webhook （如果適用）</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">建立任何必要的Webhook</a> 適合您的企業。  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">建立Webhook</a> </td>
  </tr>
</tbody>
</table>

## 寶箱 {#treasure-chest}

<table>
<thead>
  <tr>
    <th>區域</th>
    <th>動作專案</th>
    <th>優先順序</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>寶箱</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">啟用Treasure Chest</a> 以嘗試試驗功能。  <br>決定要開啟或關閉的功能。</td>
    <td>文字</td>
  </tr>
  <tr>
    <td>行銷活動檢視窗 </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">開啟行銷活動檢視窗</a> 一次檢視所有Smart Campaigns。</td>
    <td>文字</td>
  </tr>
</tbody>
</table>
