---
description: 為您新的Marketo Engage執行個體設定「管理員」區段。
title: 新執行個體最佳實務 — 管理員區段檢查清單
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: 97480487268af59aac90ef64bc1ef35ee81db310
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 新執行個體最佳實務：管理員區段檢查清單 {#new-instance-best-practices-admin-section-checklist}

身為新管理員，請套用以下檢查清單來協助引導您完成實作程式，以瀏覽全新Marketo Engage例項。 與所有這些指南一樣，您可以下載檢查清單 [連結] 並追蹤您的進度。

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色</td>
    <td><li>檢閱預先建立的角色，並確認每個角色具有的許可權/存取權。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">建立新角色</a> 或 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">編輯角色</a> 根據您組織的需求而定。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">將使用者指派給適當的角色</a>. 必須先將使用者新增至Adobe Admin Console中的訂閱，才能授與其在「角色」中的角色。 請參閱以下的「使用者」一節： <a href="/help/marketo/getting-started-2/initial-setup/user-setup.md">初始設定檢查清單</a>.</li>
    <li>為使用者指派角色後，檢閱每個角色的使用者數量。</li>
    <li>為每個API使用者實作唯一的角色，以方便疑難排解。</li></td>
  </tr>
  <tr>
    <td>文件</td>
    <td><li>為您的組織定義使用者和角色。</li>
    <li>定義新增使用者/管理員的程式。</li></td>
  </tr>
  <tr>
    <td>沙箱（如果適用）</td>
    <td><li>請檢閱上述類別中的 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙箱</a>.</li></td>
  </tr>
</tbody>
</table>

## 工作區與分割區 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作區與分割區（如果適用）</td>
    <td><li>決定數量<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> 工作區</a> 和/或分割您的組織所需的和 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">每個工作區有多少使用者有存取權。</a></li>
    <li>定義每個工作區和分割區的主要用途。</li>
    <li>定義工作區與分割區之間的關係。</li></td>
  </tr>
  <tr>
    <td>文件</td>
    <td><li>記錄工作區的定義方式以及與資料庫分割相關的方式（例如，顯示每個人相對於業務部門的全域工作區）。</li>
    <li>將新記錄匯入適當的資料分割。</li>
    <li>在您的CRM中定義值，該值會將使用者放置在適當的資料分割中。</li></td>
  </tr>
</tbody>
</table>

## Smart Campaign設定 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign設定</td>
    <td><li>新增 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">Smart Campaign大小限制</a>，防止不小心以電子郵件傳送整個資料庫。</li></td>
  </tr>
</tbody>
</table>

## 電子郵件設定 {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>電子郵件預設值</td>
    <td><li>在「品牌化網域」下，選取您的網域並新增您的電子郵件CNAME。 其格式應為： [EmailTrackingCNAME]。[CompanyDomain].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">聯絡Marketo支援</a> 透過SSL憑證布建來保護它。 此程式最多可能需要3個工作日才能完成。</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">設定SPF與DKIM</a> 以取得電子郵件傳遞能力。</li></td>
  </tr>
</tbody>
</table>

## 通訊限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通訊限制</td>
    <td><li>啟動 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">通訊限制</a>.</li>
    <li>判斷您的企業是否需要有關通訊限制的原則。</li></td>
  </tr>
</tbody>
</table>

## 標記 {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>頻道</td>
    <td><li>定義使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">管道</a>.</li></td>
  </tr>
  <tr>
    <td>標記</td>
    <td><li>定義使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">標籤</a>.</li></td>
  </tr>
  <tr>
    <td>行事曆（如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">問題行銷行事曆座位</a> 提供給需要存取許可權的使用者。</li>
    <li>設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">行事曆</a>.</li></td>
  </tr>
</tbody>
</table>

## 資料庫管理 {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>欄位管理</td>
    <td><li>實作命名慣例 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">自訂欄位</a> （例如，以「MKTO」開頭）。</li>
    <li>選擇您同步的欄位。 您同步的欄位越多，同步週期就越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">封鎖欄位更新</a> 您想要寫入一次（例如，原始銷售機會來源、原始銷售機會來源詳細資料、首次接觸UTM欄位等）。</li></td>
  </tr>
  <tr>
    <td>自訂活動</td>
    <td><li>定義 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">自訂活動</a> 特定於您的企業。</li></td>
  </tr>
  <tr>
    <td>自訂物件</td>
    <td><li>檢視數量 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">自訂物件</a> 您需要。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">將這些自訂物件同步至您的CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## 整合 {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>起始CRM同步。 請根據貴公司使用的CRM從下列專案中選擇： <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>識別存取CRM所需的存取權型別。</li>
    <li>識別您的CRM管理員以進行疑難排解。</li></td>
  </tr>
  <tr>
    <td>網站服務</td>
    <td><li>決定可以製作的使用者/應用程式 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">API呼叫</a> 在您的例項中。</li>
    <li>檢閱將進行API呼叫的所有應用程式，並判斷是否需要增加或減少API呼叫。</li></td>
  </tr>
  <tr>
    <td>啟動點</td>
    <td><li>設定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">啟動點</a> 為貴企業提供的服務。 每個LaunchPoint都應搭配唯一的API使用者，以協助疑難排解。</li></td>
  </tr>
  <tr>
    <td>互動式網路研討會（如適用）</td>
    <td>注意：互動式網路研討會只會布建至生產執行個體。
    <li>對於建立互動式網路研討會，內建的網路研討會功能， <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">將使用者新增至「使用者」區段</a> 在互動式網路研討會標籤上。</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（如果適用）</td>
    <td><li>將使用者指派至 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">「存取Dynamic Chat」角色</a> 在「Marketo Engage&gt;管理員&gt;使用者和角色」中。</li></td>
  </tr>
  <tr>
    <td>銷售分析（如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">設定銷售分析動作</a> 「銷售分析&gt;動作設定」中的。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">將名額發給適當的使用者</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">設定API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">自訂潛在客戶分數</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect （如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">邀請適當的Marketo Engage管理員加入Sales Connect執行個體</a>.</li>
    <li>完成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">其他Sales Connect管理員設定</a> Sales Connect和Salesforce中的。</li></td>
  </tr>
  <tr>
    <td>Webhook （如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">建立任何必要的Webhook</a> 適合您的企業。</li>
    </td>
  </tr>
</tbody>
</table>

## 寶箱 {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>寶箱 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">啟用Treasure Chest</a> 以嘗試試驗功能。</li>
    <li>決定要開啟或關閉的功能。</li></td>
  </tr>
  <tr>
    <td>行銷活動檢視窗 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">開啟行銷活動檢視窗</a> 一次檢視所有Smart Campaigns。</li></td>
  </tr>
</tbody>
</table>
