---
description: 為您新的Marketo Engage執行個體設定「管理員」區段。
title: 新執行個體最佳實務 — 管理員區段檢查清單
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---

# 新執行個體最佳實務：管理員區段檢查清單 {#new-instance-best-practices-admin-section-checklist}

身為新管理員，請套用以下檢查清單來協助引導您完成實作程式，以便瀏覽全新的Marketo Engage執行個體。 與所有這些指南一樣，您也可以[下載檢查清單](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)並追蹤進度。

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色</td>
    <td><li>檢閱預先建立的角色，並確認每個角色具有的許可權/存取權。</li>
    <li>根據您組織的需求<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=zh-Hant#create-a-new-role" target="_blank">建立新角色</a>或<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=zh-Hant#edit-a-role" target="_blank">編輯角色</a>。</li>
    <li><a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">將使用者指派給適當的角色</a>。 必須先將使用者新增至Adobe Admin Console中的訂閱，才能在「角色」中授予其角色。 請參閱<a href="/help/marketo/getting-started/initial-setup/user-setup.md">初始設定檢查清單</a>中的「使用者」區段。</li>
    <li>為使用者指派角色後，檢閱每個角色的使用者數量。</li>
    <li>為每個API使用者實作唯一的角色，以方便疑難排解。</li></td>
  </tr>
  <tr>
    <td>沙箱（如果適用）</td>
    <td><li>檢閱上述<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙箱</a>的類別。</li></td>
  </tr>
</tbody>
</table>

## 工作區與分割區 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作區與分割區（如果適用）</td>
    <td><li>決定您的組織需要擁有的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=zh-Hant" target="_blank">工作區數目</a>和/或分割區，以及<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=zh-Hant" target="_blank">每個工作區有多少使用者可以存取。</a></li>
    <li>定義每個工作區和分割區的主要用途。</li>
    <li>定義工作區與分割區之間的關係。</li></td>
  </tr>
</tbody>
</table>

## Smart Campaign設定 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign設定</td>
    <td><li>在Smart Campaign大小<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=zh-Hant" target="_blank">上新增</a>限制，以防止不小心寄送電子郵件給整個資料庫。</li></td>
  </tr>
</tbody>
</table>

## 通訊限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通訊限制</td>
    <td><li>實作<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=zh-Hant" target="_blank">通訊限制</a>。</li>
    <li>判斷您的企業是否需要有關通訊限制的原則。</li></td>
  </tr>
</tbody>
</table>

## 標記 {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>管道</td>
    <td><li>定義如何使用<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=zh-Hant" target="_blank">管道</a>。</li></td>
  </tr>
  <tr>
    <td>標記</td>
    <td><li>定義如何使用<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=zh-Hant" target="_blank">標籤</a>。</li></td>
  </tr>
  <tr>
    <td>行事曆<br>
    （如果適用）</td>
    <td><li>將行銷行事曆名額<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=zh-Hant" target="_blank">問題</a>給需要存取權的使用者。</li>
    <li>設定<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=zh-Hant" target="_blank">行事曆</a>。</li></td>
  </tr>
</tbody>
</table>

## 資料庫管理 {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>欄位管理</td>
    <td><li>實作<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=zh-Hant" target="_blank">自訂欄位</a>的命名慣例（例如，以「MKTO」開頭）。</li>
    <li>選擇您同步的欄位。 您同步的欄位越多，同步週期就越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=zh-Hant" target="_blank">封鎖更新至您要寫入一次的欄位</a> （例如，原始潛在客戶來源、原始潛在客戶來源詳細資料、首次接觸UTM欄位等）。</li></td>
  </tr>
  <tr>
    <td>自訂活動</td>
    <td><li>定義您企業專屬的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=zh-Hant" target="_blank">自訂活動</a>。</li></td>
  </tr>
  <tr>
    <td>自訂物件</td>
    <td><li>檢閱您需要的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=zh-Hant" target="_blank">自訂物件</a>數目。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=zh-Hant" target="_blank">將這些自訂物件</a>同步至您的CRM。</li></td>
  </tr>
</tbody>
</table>

## 整合 {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>識別存取CRM所需的許可權。</li>
    <li>識別您的CRM管理員以進行疑難排解。</li></td>
  </tr>
  <tr>
    <td>網站服務</td>
    <td><li>決定可在您的執行個體中進行<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=zh-Hant" target="_blank">API呼叫</a>的使用者/應用程式。</li>
    <li>檢閱將進行API呼叫的所有應用程式，並判斷是否需要增加或減少API呼叫。</li></td>
  </tr>
  <tr>
    <td>啟動點</td>
    <td><li>為您的企業設定<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=zh-Hant" target="_blank">LaunchPoint</a>服務。 每個LaunchPoint都應搭配唯一的API使用者，以協助疑難排解。</li></td>
  </tr>
  <tr>
    <td>互動式網路研討會（如適用）</td>
    <td><li>若要建立互動式網路研討會，請使用Marketo Engage內建的網路研討會功能，<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">將使用者新增至互動式網路研討會標籤上的「使用者」區段</a>。</li>
    <p><img src="assets/note-icon.png" alt="附註圖示"> 注意：互動式網路研討會只會布建至生產執行個體。</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat （如果適用）</td>
    <td><li>在Marketo Engage &gt;管理員&gt;使用者和角色中，將使用者指派給<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">'存取Dynamic Chat的角色</a>。</li></td>
  </tr>
  <tr>
    <td>銷售Insight （如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">在銷售Insight &gt;動作設定中設定銷售Insight動作</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=zh-Hant#invite-individual-users-to-msi-actions" target="_blank">將名額</a>發給適當的使用者。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=zh-Hant" target="_blank">設定API</a>。</li>
    <li>自訂<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=zh-Hant" target="_blank">潛在客戶分數</a>。</li></td>
  </tr>
  <tr>
    <td>Sales Connect （如果適用）</td>
    <td><li>邀請適當的Marketo Engage管理員加入<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect執行個體</a>。</li>
    <li>完成Sales Connect和Salesforce中的<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">其他Sales Connect管理員設定</a>。</li></td>
  </tr>
  <tr>
    <td>Webhook （如果適用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=zh-Hant" target="_blank">為您的企業建立任何必要的Webhook</a>。</li>
    </td>
  </tr>
</tbody>
</table>

## 寶箱 {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>寶箱 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=zh-Hant" target="_blank">啟用Treasure Check</a>，嘗試試用功能。</li>
    <li>決定要開啟或關閉的功能。</li></td>
  </tr>
  <tr>
    <td>行銷活動檢視窗 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=zh-Hant" target="_blank">開啟Campaign Inspector</a>，在一個位置檢視您所有的Smart Campaign。</li></td>
  </tr>
</tbody>
</table>
