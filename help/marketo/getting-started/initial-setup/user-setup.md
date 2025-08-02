---
description: 在深入使用新的 Marketo Engage 執行個體之前，您需要完成一些基本步驟才能持續使用。這些步驟包括使用者帳戶設定、支援管理員設定以及訂閱持續的系統更新。
short-description: 完成初步設定步驟後，了解如何建立基本元素以確保順利持續使用。
title: 使用者設定檢查清單
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 7%

---

# 使用者設定檢查清單 {#user-setup-checklist}

現在您已完成所有[初始設定步驟](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}，您可以建立一些基礎元素，以確保順利進行使用。 這將為您的使用Marketo Engage的歷程奠定基礎，並幫助您充分利用其功能。 我們開始吧！

>[!NOTE]
>
>您也可以下載此檢查清單[以及您新執行個體的最佳實務清單](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)，並隨時檢視這些步驟。

## Adobe Identity Management上的Marketo Engage {#marketo-engage-on-adobe-identity-management}

您的新Marketo Engage訂閱已上線到[Adobe Identity Management系統(IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=zh-Hant)。 繼續下列在Adobe Admin Console中的使用者管理檢閱。

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>訂閱與Marketo Engage產品管理員</td>
    <td><li>確認您的Adobe組織系統管理員已授予您Adobe產品管理員角色。</li>
    <ul>
    <li>請連絡Adobe客戶團隊（您的客戶經理）或傳送電子郵件至<code>marketocares@marketo.com</code>，以瞭解貴組織中的哪些人員擁有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=zh-Hant">Adobe Admin Console系統管理員</a>許可權。</li></ul>
    <li>接受「Marketo Engage產品管理員」邀請以啟用您的Adobe ID。 在Adobe Admin Console中指派角色時會傳送<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=zh-Hant#create-a-product-profile">歡迎電子郵件</a>。</li></td>
  </tr>
  <tr>
    <td>產品設定檔</td>
    <td><li>在Adobe Admin Console中指派所有所需使用者至Marketo Engage <a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">產品設定檔</a>。</li>
    <ul>
    <li>將使用者新增至產品設定檔之前，您無法在「Marketo Engage &gt;管理員&gt;使用者和角色」中指派使用者角色。</li>
    <li>每個訂閱都將是獨立的產品設定檔。 如果將不需要的使用者新增到多個產品設定檔（例如，生產和測試沙箱），您必須從所有產品設定檔中刪除該使用者。 否則，他們仍可存取Marketo Engage。</li></ul></td>
  </tr>
  <tr>
    <td>使用者</td>
    <td><li>建立原則於何時<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html?lang=zh-Hant">建立使用者</a>。</li> <li>在何時移除使用者時建立原則。</li>
    <p><img src="assets/note-icon.png" alt="附註圖示"> 注意：您必須是系統管理員才能移除使用者。
    <li>決定應該擁有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=zh-Hant">Adobe系統管理員和Marketo Engage產品管理員許可權的使用者。</a> <li><a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">將使用者</a>新增到所需的產品設定檔。</li>
    <li>為每個API使用案例建立一個API使用者。</li></td>
  </tr>
  <tr>
    <td>User Management API （如果適用）</td>
    <td><li>使用<a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe使用者管理API</a>來邀請、更新及刪除使用者。</li>
    <li>使用<a href="https://developer.adobe.com/umapi/">Adobe使用者管理API</a>新增或移除角色（例如管理員、支援管理員、開發人員）。</li>
    </td>
  </tr>
  <tr>
    <td>產品支援管理員</td>
    <td><li>若要<a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=zh-Hant#create-a-support-ticket-with-admin-console">在Adobe Admin Console</a>中提交支援票證，您必須擁有系統管理員為您管理的訂閱指派的「產品支援管理員」角色。 只有您組織中的系統管理員可以<a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=zh-Hant#assign-the-support-admin-role">將您</a>指派給此角色。</li>
    <li>您可能會收到系統管理員的電子郵件，告知您是您Marketo Engage訂閱的支援管理員。 若是如此，請按一下電子郵件中的<a href="https://experienceleague.adobe.com/zh-hant/docs/customer-one/using/home#assign-the-support-admin-role">[開始使用]</a>以加入組織。</li>
    <li>決定適當的連絡人（至少要有一個備用連絡人），並要求系統管理員指派相應的產品支援管理員角色。</li></td>
  </tr>
</tbody>
</table>

## Adobe上的Dynamic Chat Identity Management設定 {#dynamic-chat-on-adobe-identity-management}

若要使用Marketo Engage中的原生交談自動化管道[Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=zh-Hant)，請依照下列[Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}中的步驟繼續進行使用者許可權設定。

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>訂閱與Dynamic Chat產品管理員（如果適用）</td>
    <td><li>確認您的Adobe組織系統管理員已授予您Adobe產品管理員角色。</li>
    <ul><li>請連絡Adobe客戶團隊（您的客戶經理）或傳送電子郵件至<code>marketocares@marketo.com</code>，以瞭解貴組織中的哪些人員擁有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=zh-Hant">Adobe Admin Console系統管理員</a>許可權。</li></ul>
    <li>接受<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=zh-Hant">'Dynamic Chat產品管理員'</a>邀請。 在您的Marketo Engage執行個體中啟用Dynamic Chat並且您被指定為系統管理員時，會傳送<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=zh-Hant">歡迎電子郵件</a>。</li></td>
  </tr>
  <tr>
    <td>產品設定檔</td>
    <td><li>將所有所需使用者指派給Adobe Admin Console中的Dynamic Chat產品設定檔。</li>
    <ul>
    <li>如果將不需要的使用者新增到多個產品設定檔，您必須從所有產品設定檔中刪除該使用者。 否則，他們仍可存取Dynamic Chat。</li>
    <li>您可以<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">在Dynamic Chat中編輯產品設定檔</a>，並使用您的訂閱<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">中可用的自訂許可權集</a>建立自訂設定檔。</li></td>
  </tr>
  <tr>
    <td>使用者</td>
    <td><li>在何時新增和移除聊天使用者上建立原則。</li>
    <li>建立應該擁有<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat產品管理員許可權的原則。</a></li>
    <li><a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">將使用者新增至所需的產品設定檔</a>。</li></td>
  </tr>
</tbody>
</table>

## 設定持續的系統更新與通訊 {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Marketo狀態更新</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">訂閱Adobe Marketo Engage狀態更新</a>。</li></td>
  </tr>
  <tr>
    <td>通知</td>
    <td><li><a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">訂閱管理員通知</a>以取得重大問題，例如您的智慧行銷活動發生錯誤，以及CRM同步處理發現的重大問題。</li></td>
  </tr>
</tbody>
</table>

<p>

現在您的Marketo Engage帳戶已準備就緒，請檢閱新的Marketo Engage執行個體的[最佳實務](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"}區段，以充分利用您的投資，並為長期成功做好準備。
