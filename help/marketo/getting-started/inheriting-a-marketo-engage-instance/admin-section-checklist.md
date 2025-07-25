---
description: 繼承執行個體管理員檢查清單 — Marketo檔案 — 產品檔案
title: 繼承執行個體管理員檢查清單
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# 繼承執行個體：管理員區段檢查清單 {#inherited-instance-admin-section-checklist}

Adobe Professional Services已將以下核對清單（連結至每篇文章底部的後續核對清單）與Marketo Champions的輸入彙整在一起，協助您快速上手。 您也可以[下載檢查清單](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)並追蹤進度。

>[!TIP]
>
>如果您是Marketo Engage的新使用者，且不熟悉許多術語，請檢視[Marketo Engage字彙表](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}。

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>這僅適用於上架到[Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}的Marketo Engage訂閱。 如果您的訂閱尚未上線Adobe IMS，請在「Marketo Engage >管理員>使用者和角色」中繼續進行[舊版使用者角色和許可權體驗](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}。

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th> 
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>訂閱與Marketo Engage產品管理員</td> 
   <td><li>您的Marketo Engage訂閱是否已移轉至<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a>？ 
<br/>     若是如此，您的「Adobe Admin Console系統管理員」是否已授予您「Adobe Admin Console產品管理員」角色？ 如果您不確定組織中的哪些人擁有主控台中的管理員許可權，請聯絡<a href="https://helpx.adobe.com/tw/contact.html" target="_blank">Adobe客戶服務</a>。</li>
<li>您是否接受「Marketo Engage產品管理員」邀請？ 在Adobe Admin Console中指派角色時，會傳送電子郵件。
<br/>     如果沒有，請在收件匣中尋找<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">歡迎電子郵件</a>，並接受邀請以啟用您的Adobe ID。</li></td>
  </tr>
  <tr> 
   <td>產品設定檔</td> 
   <td><li>在Adobe Admin Console中，是否已將所有適當的使用者指派給Marketo Engage的產品設定檔？
<br/>     如果沒有，請確定<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">在Adobe Admin Console中，從Marketo Engage產品設定檔新增和/或移除使用者</a>。 如果您將使用者新增至產品設定檔，您無法在「Marketo Engage &gt;管理員&gt;使用者和角色」中指派使用者。</li>
<p><img src="assets/note-icon.png" alt="附註圖示"> 注意：如果將不需要的使用者新增到多個產品設定檔，您必須從所有產品設定檔中移除該使用者。 否則，他們仍可存取Marketo Engage。</td>
  </tr>
  <tr> 
   <td>使用者管理API</td> 
   <td><li>您的訂閱使用任何Marketo User Management API嗎？
<br/>     若是如此，您必須使用<a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS API</a>，才能邀請、更新及刪除日後使用者。</li>
<p><img src="assets/note-icon.png" alt="附註圖示"> 注意：「角色管理」仍保留在Marketo Engage中，而Marketo使用者管理API仍可用於角色管理。</td>
  </tr>
 </tbody> 
</table>

## 使用者和角色 {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td><img src="assets/note-icon.png" alt="附註圖示"> 注意：如果您的訂閱已位於Adobe IMS，請繼續進行Adobe Admin Console中的下列使用者管理檢閱。 否則，請前往Marketo Engage中的「管理員&gt;使用者和角色&gt;使用者」 。
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">有多少使用者</a>？</li>
<li>是否有任何應<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">移除</a>的使用者？</li>
<li>貴公司是否有刪除使用者的相關政策？</li> 
<li>有多少使用者擁有<a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理員許可權</a>？</li>
<li>這些使用者中應該有任何變更為<a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">其他角色嗎？</a></li> 
<li>誰是此執行個體中的<a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API使用者</a>？</li></td>
  </tr>
  <tr> 
   <td>角色</td> 
   <td><img src="assets/note-icon.png" alt="附註圖示"> 注意：無論您是否將Marketo與Adobe身分搭配使用，請繼續在「管理員&gt;使用者和角色&gt;角色」底下檢閱Marketo Engage中的角色許可權。
   <p><li>有多少角色？</li>  
<li>每個角色都有哪些<a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">許可權/存取權</a>？ 是否應對任何專案進行調整？</li>
<li>每個角色有多少使用者？</li>
<li>使用者<a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">登入</a>的頻率為何？</li>
<li>每個API使用者是否有自己的<a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">使用者角色</a>？ 如果不能，請考慮實作此專案以更輕鬆進行疑難排解。</li> 
<li>您的使用者角色和許可權是否符合法規遵循的企業資料隱私權政策（例如<a href="https://gdpr-info.eu/" target="_blank">GDPR</a>）？ 公司資料<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">隱私權原則</a>是否允許使用者下載及共用Marketo Engage使用者資料？ 需要許可業務嗎？</li></td>
  </tr>
  <tr> 
   <td>支援使用者</td> 
   <td><li>您是否在支援入口網站中設定適當的<a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">授權連絡人</a>？</li></td>
  </tr>
  <tr> 
   <td>內部檔案</td> 
   <td><li>貴組織中是否清楚定義使用者和角色？</li>
<li>您新增使用者/管理員的程式為何？</li></td>
  </tr>
  <tr> 
   <td>沙箱（如果適用）</td> 
   <td><li>您有<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙箱執行個體</a>嗎？
   <br/>     如果是這樣的話，請檢閱上述適用於您的沙箱的類別。</li>
<li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">程式匯入</a>是否連結至您的沙箱？</li></td>
  </tr>
 </tbody> 
</table>

## 稽核軌跡 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>稽核軌跡</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">執行個體中誰正在工作</a>？</li></td>
  </tr>
 </tbody> 
</table>

## 工作區與分割區 {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>工作區與分割區</td> 
   <td><li>您有多少<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">工作區和/或分割區</a>？</li>
<li>每個Workspace和分割的主要用途為何？</li>
<li>您的<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">工作區</a>或<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">分割區</a>是否需要稽核/變更？</li>
<li>您的工作區與資料分割之間的關係為何？</li>
<li><a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">有多少使用者擁有每個Workspace的存取權</a>？</li></td>
  </tr>
  <tr> 
   <td>內部檔案</td> 
   <td><li>如何定義工作區和分割區？</li>
<li>將Workspaces新增至您的執行個體或新增使用者至Workspace的程式為何？</li></td>
  </tr>
 </tbody> 
</table>

## Smart Campaign {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>Smart Campaign</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">您對Smart Campaign的大小是否有限制</a>？ 
   <br/>     如果沒有，請考慮新增一個。 我們建議將Smart Campaign限制限製為資料庫的25%，以避免在工作流程中過度通訊或處理整個資料庫；這不僅可保護您的品牌，還有助於保護執行個體的效能。</li></td>
  </tr>
 </tbody> 
</table>

## 通訊限制 {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>通訊限制</td> 
   <td><li>是否有<a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">通訊限制</a>？ 貴企業是否有可能需要通訊限制的原則？</li>
<p><img src="assets/note-icon.png" alt="附註圖示"> 注意：我們建議將通訊限製為每天1封，每7天3封，並封鎖<b>非</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">可運作</a>封電子郵件。</td>
  </tr>
 </tbody> 
</table>

## 標記 {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>標記</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">有多少標籤</a>？ 目前使用多少個標籤？ 是否需要新增？</li>
<li>您的程式是否需要標籤？</li></td>
  </tr>
  <tr> 
   <td>管道</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">有多少管道</a>？ 目前使用多少個？</li>
<li>所有<a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">頻道方案狀態是否適當</a>？ 它們是否在計畫中顯示進度？</li>
<li>您的管道是否與特定計畫型別有關？</li>
<li>每個管道的哪些狀態被視為成功？ 這些是否符合您的行銷目標？</li>
<li>是否正確使用營運管道？</li>
<li>針對進階Report Builder （收入週期總管/RCE），您的管道分析行為是否設定為符合納入期間成本的方案實務？</li></td>
  </tr>
  <tr> 
   <td>行銷行事曆（如果適用）</td> 
   <td><li>有多少<a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">行事曆專案型別</a>？ 它們是否仍然相關？</li></td>
  </tr>
 </tbody> 
</table>

## 資料庫管理 {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>欄位管理</td> 
   <td><li>有多少欄位？ 
   <br/>     按一下<a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">匯出欄位名稱</a>以檢閱您的欄位、自訂欄位及其API名稱的清單。</li>
<li>有多少<a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">個自訂欄位</a>？</li>
<li>使用了多少欄位？ 
<br/>     選取[欄位動作]下拉式清單中的[匯出使用者]，以檢閱欄位的相關資產。<a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank"></a></li>
<li>Marketo Engage與您的CRM之間同步了多少欄位？</li>
<li>CRM欄位是否已同步至適當的物件？</li>
<li>人員詳細資料是否有<a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">自訂檢視集</a>？ 應該有嗎？</li>
<li>根據來源，您的欄位是否有命名慣例？ 
<br/>     如果沒有，請考慮實作此專案。</li>
<li>是否有任何欄位<a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">已封鎖</a>？ 
<br/>     若是如此，請務必瞭解原因。</li></td>
  </tr>
  <tr> 
   <td>自訂活動</td> 
   <td><li>是否有任何<a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">自訂活動</a>？
<br/>     若是如此，請按一下這些欄位，瞭解哪些活動與Marketo表單、電子郵件或登入頁面無關。</li></td>
  </tr>
  <tr> 
   <td>自訂物件</td> 
   <td><li>有多少<a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">個自訂物件</a>？ 他們如何同步至您的CRM？</li>
<li>您的程式和清單查詢如何使用這些自訂物件？</li></td>
  </tr>
 </tbody> 
</table>

## 電子郵件 {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>電子郵件預設設定</td> 
   <td><li>在「管理員&gt;電子郵件」中，所有預設設定都是最新狀態（例如，<a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">「來自」電子郵件/標籤</a>、<a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">品牌化網域</a>、<a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">取消訂閱訊息</a>等）？</li></td>
  </tr>
 </tbody> 
</table>

## 整合 {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>您正在同步至哪個CRM？ Salesforce？ MS Dynamics？ 維耶娃？</li>
<li>您是否正在使用<a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">自訂同步處理</a>？</li>
<li>[僅限Salesforce]您的執行個體是否已實作自訂同步篩選器？ 
<p><img src="assets/note-icon.png" alt="附註圖示"> 注意：請聯絡Marketo支援以識別自訂同步篩選器，或要求實作自訂同步規則。</li></td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td><li>什麼是<a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">網域設定為</a>？</li>
   <li>首頁設定為何？</li>
<li><a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">遞補集為</a>是什麼？</li>
<li>是否啟用表單預填？</li>
<li><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">個人化URL</a>是否已啟用？</li>
<li>是否已為<a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">重新導向</a>設定規則？</li>
<li>您有設定好的網域別名嗎？ 您是否追蹤您使用網域別名的方式？</li>
<li>登陸頁面</a>的<a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">安全網域是否已啟用？ 
<br/>     確認您的登入頁面資產是否包含「http」URL。</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>您的<a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin追蹤代碼</a>是否在您的網站上(不是Marketo Engage登陸頁面)？</li>
<li><a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track</a>瀏覽器請求是否已啟用？</li>
<li>是否已設定您的<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking" target="_blank">Munchkin API</a>？ 
<p><img src="assets/tip-icon.png" alt="提示圖示">提示：如果您遺失munchkin程式碼在您網站上的位置檔案，您可以建立<a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">網頁活動報告</a>來檢視所有URL。</li></td>
  </tr>
  <tr> 
   <td>網站服務</td> 
   <td><li>是否啟用<a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP限制</a>？ 他們應該是？</li>
<li>哪些使用者/應用程式正在您的執行個體中進行API呼叫？</li>
<li>您是否達到或接近達到API限制？
<br/>     如果是這樣的話，請考慮增加此功能或稽核您的執行個體，以叫停這些API呼叫。</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat （如果適用）</td> 
<td>若要遵循下列步驟，必須存取<a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>。 如果您尚未設定Adobe ID，請<a href="https://helpx.adobe.com/tw/manage-account/using/create-update-adobe-id.html" target="_blank">在這裡瞭解如何設定</a>。
<br/>
<li>您是否接受<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Dynamic Chat產品管理員</a>邀請？ 電子郵件會在您的Marketo Engage執行個體中啟用Dynamic Chat時傳送，而且您會指定為系統管理員。
<br/>     如果沒有，請在收件匣中尋找歡迎電子郵件，並接受邀請以設定您的Adobe ID。</li>   
<li>您是否已將<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">所要的使用者</a>新增至Adobe Admin Console中的Dynamic Chat產品設定檔？
<li>請確認符合資格的使用者已將其Dynamic Chat產品設定檔新增至其Adobe身分識別中。 如果您已將「存取Dynamic Chat」角色新增至產品設定檔，您無法在「Marketo Engage &gt;管理員&gt;使用者和角色」中指派這些角色。</li>
<li>在「產品設定檔」索引標籤中，預設設定檔許可權是否符合您組織的需求？<br/> 
如果沒有，請編輯特定設定檔的許可權。 </li>
<li>如果您有多個訂閱，您的使用者是否會新增至正確的訂閱？</li>
<br>
完成稽核使用者與角色設定後，請登入Dynamic Chat以繼續稽核。  
<li>您<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">已將您的Marketo Engage執行個體</a>連線至Dynamic Chat嗎？</li>
<li>具有預先定義許可權的五個預設設定檔是否適用於您的組織？<br/> 
     如果沒有，您可以<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">在Dynamic Chat中編輯它們</a>。 您也可以<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">建立具有自訂許可權集的自訂設定檔</a>。</li>
<li>若要讓使用者存取Dynamic Chat，您已核取「管理員&gt;使用者和角色&gt;角色」中適用的Marketo Engage角色的「存取Dynamic Chat」嗎？
<br/><img src="assets/note-icon.png" alt="附註圖示">注意：「管理員」和「行銷使用者」角色應該要能存取Dynamic Chat。</li>
</td>
  </tr>
  <td>Marketo Sales Insight （如果適用）</td> 
   <td><li>是否已安裝<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI封裝</a>？</li>
<li>您<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">已升級至最新版的Sales Insight</a>嗎？</li>
<li>您是否已完成Sales Insight設定？ <br/>     Enterprise/Unlimited使用者<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">按一下這裡</a>，Professional使用者<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">按一下這裡</a>。</li>
<li>您是否已根據您購買的座位數<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">為您的使用者</a>授予存取權？</li>
<li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">星和火焰</a>是否已自訂？</li></td>
  </tr>
  <tr> 
   <td>啟動點（如果適用）</td> 
   <td><li>您設定了哪些服務（例如<a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>、<a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>等）？ 是否有任何已接近其有效期的專案？</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">您的整合使用多少API呼叫</a>？</li>
<li>您是否已為使用案例制定正確的整合？</li></td>
  </tr>
  <tr> 
   <td>Webhook （如果適用）</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">您設定了哪些連線</a>？</li>
<li>任何已不再使用嗎？</li></td>
  </tr>
  <tr> 
   <td>行動應用程式（如適用）</td> 
   <td><li>您有哪些<a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">行動應用程式</a>？</li>
<li>是否已新增任何<a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">測試裝置</a>？</li></td>
  </tr>
 </tbody> 
</table>

## 寶箱 {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>寶箱</td> 
   <td><li><a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">寶藏箱</a>中開啟了什麼功能？</li>
<li>是否有應開啟或關閉的功能？</li></td>
  </tr>
  <tr> 
   <td>行銷活動檢視窗</td> 
   <td><li><a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">行銷活動檢視窗</a>是否已開啟？
<br/>如果沒有，請考慮開啟以輕鬆識別哪些促銷活動：作用中、與您的CRM同步，以及/或刪除記錄。</li></td>
  </tr>
 </tbody> 
</table>

## 警示和更新 {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">區域圖</th>
   <th>評論焦點</th>
  </tr> 
  <tr> 
   <td>Marketo Engage狀態更新</td> 
   <td><li>您的執行個體是否已訂閱<a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage狀態更新</a>？</li></td>
  </tr>
  <tr> 
   <td>警報</td> 
   <td><li>是否有任何<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">作用中警示</a>從Marketo Engage傳送給內部團隊？</li>
<li>如果有的話，這些警報是否可正常運作？</li></td>
  </tr>
  <tr> 
   <td>通知</td> 
   <td><li>您是否已訂閱適當的管理員<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">通知</a>？</li></td>
  </tr>
 </tbody> 
</table>
