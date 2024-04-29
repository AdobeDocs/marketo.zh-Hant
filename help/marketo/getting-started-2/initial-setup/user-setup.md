---
description: 開始使用新的Marketo Engage執行個體前，您需要完成一些基礎步驟才能繼續使用。 這些步驟包括使用者帳戶設定、支援管理員設定，以及訂閱進行中的系統更新。
title: 使用者設定檢查清單
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: f9bf2082968737277b3c976659802992f975ec9a
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# 使用者設定檢查清單 {#user-setup-checklist}

現在您已完成所有 [初始設定任務](/help/marketo/getting-started-2/initial-setup/initial-setup-tasks.md)，現在應該建立一些基礎元素，以確保順暢的持續使用。 這將為您使用Marketo Engage的旅程奠定基礎，並幫助您充分利用其功能。 讓我們開始吧！

>[!NOTE]
>
>您也可以下載檢查清單 [插入連結] 並立即檢視步驟。

## 在AdobeIdentity Management上Marketo Engage {#marketo-engage-on-adobe-identity-management}

您的新Marketo Engage訂閱已上線到 [AdobeIdentity Management系統(IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). 繼續下列在Adobe Admin Console中的使用者管理檢閱。

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>訂閱和Marketo Engage產品管理員 </td>
    <td><li>確認您的Adobe組織系統管理員已授予您Adobe產品管理員角色。</li>  
    <ul>
    <li>連絡人 <a href="https://helpx.adobe.com/contact.html">Adobe客戶服務</a> 以找出貴組織中的人員 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console系統管理員</a> 許可權。</li></ul>
    <li>接受「Marketo Engage產品管理員」邀請以啟用您的Adobe ID。 此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">歡迎電子郵件</a> 在Adobe Admin Console中指派角色時傳送。</li></td>
  </tr>
  <tr>
    <td>產品設定檔</td>
    <td><li>將所有所需使用者指派給Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">產品設定檔</a> 在Adobe Admin Console中。</li>
    <ul>
    <li>將使用者新增至產品設定檔之前，您無法在「Marketo Engage&gt;管理員&gt;使用者與角色」中指派使用者角色。</li>
    <li>每個訂閱都將是獨立的產品設定檔。 如果將不需要的使用者新增到多個產品設定檔（例如，生產和測試沙箱），您必須從所有產品設定檔中刪除該使用者。 否則，他們仍可存取Marketo Engage。</li></ul></td>
  </tr>
  <tr>
    <td>使用者</td>
    <td><li>建立何時執行的原則 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">建立使用者</a>.</li> <li>在何時移除使用者時建立原則。</li>
    <li>決定誰應該擁有 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe系統管理員和Marketo Engage產品管理員許可權。</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">新增使用者</a> 至所需的產品設定檔。</li>
    <li>為每個API使用案例建立一個API使用者。</li></td>
  </tr>
  <tr>
    <td>產品支援管理員 </td>
    <td><li>至 <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">在Adobe Admin Console中提交支援票證</a>，您需要由系統管理員為您管理的訂閱指派「產品支援管理員」角色。 只有您組織中的系統管理員可以 <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">將您指派給此角色</a>.</li>
    <li>您可能會收到系統管理員的電子郵件，說明您是您Marketo Engage訂閱的支援管理員。 若是如此，請按一下 <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'開始使用'</a> 加入組織的電子郵件中。</li>
    <li>決定適當的連絡人（至少要有一個備用連絡人），並要求系統管理員指派相應的產品支援管理員角色。</li></td>
  </tr>
</tbody>
</table>

## AdobeIdentity Management設定的Dynamic Chat {#dynamic-chat-on-adobe-identity-management}

使用 [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html)，此為Marketo Engage的原生交談自動化頻道，請依照以下的 [Adobe Admin Console](https://adminconsole.adobe.com/).

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>訂閱和Dynamic Chat產品管理員（如果適用） </td>
    <td><li>確認您的Adobe組織系統管理員已授予您Adobe產品管理員角色。 連絡人 <a href="https://helpx.adobe.com/contact.html">Adobe客戶服務</a> 以找出貴組織中哪些人擁有主控台中的管理員許可權。</li>
    <li>接受 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">'Dynamic Chat產品管理員'</a> 邀請。 此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">歡迎電子郵件</a> 會在您的Marketo Engage執行個體中啟用Dynamic Chat且您被指定為系統管理員時傳送。</li></td>
  </tr>
  <tr>
    <td>產品設定檔 </td>
    <td><li>將所有所需使用者指派給Adobe Admin Console中的Dynamic Chat產品設定檔。</li> 
    <ul>
    <li>如果將不需要的使用者新增到多個產品設定檔，您必須從所有產品設定檔中刪除該使用者。 否則，他們仍可存取Dynamic Chat。</li>
    <li>您可以 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">在Dynamic Chat中編輯產品設定檔</a> 並使用自訂設定檔集建立自訂設定檔 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">您的訂閱中可用的許可權</a>.</li></td>
  </tr>
  <tr>
    <td>使用者 </td>
    <td><li>在何時新增和移除聊天使用者上建立原則。</li>
    <li>建立應該讓誰擁有的原則 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat產品管理員許可權。</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">將使用者新增到所需的產品設定檔</a>.</li></td>
  </tr>
</tbody>
</table>

## 設定持續的系統更新與通訊 {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">區域</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>AdobeMarketo狀態更新 </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">訂閱Adobe Marketo Engage狀態更新消息</a>.</li></td>
  </tr>
  <tr>
    <td>通知 </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">訂閱管理員通知</a> Smart Campaigns中的錯誤，以及CRM同步作業發現的重大問題等嚴重問題。</li></td>
  </tr>
</tbody>
</table>

<p>

現在您的Marketo Engage帳戶已可供使用，請檢視我們的 [新Marketo Engage例項的最佳作法](/help/marketo/getting-started-2/implementing-a-new-marketo-engage-instance/where-to-start.md) 區段來充分利用您的投資，並為長期成功做好準備。
