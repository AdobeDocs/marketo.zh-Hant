---
description: 繼承檔案1 - Marketo檔案 — 產品檔案
title: 繼承檔案1
hide: true
hidefromtoc: true
source-git-commit: b06d1d0f8101895ebefeb821150090aac3044870
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 3%

---

# 繼承檔案1 {#inherit-doc-1}

稽核繼承的執行個體可能看起來像是……

您是否從其他管理員繼承了現有的Marketo Engage執行個體？ 若是如此，本文僅供您參考……

以下檢查清單已與Marketo Champions的輸入一併輸入，可幫助您在繼承執行個體中快速上手……

>[!TIP]
>
>如果您是新的Marketo Engage使用者，且不熟悉許多術語，請檢視 [Marketo字彙表](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## 使用者和角色 {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">使用者數量</a> 有嗎？</li>
<li>是否有任何應過期的使用者？</li>
<li>貴公司是否有刪除使用者的相關政策？</li> 
<li>使用者數量 <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理員許可權</a>？</li>
<li>這些使用者中是否應該有任何變更為 <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">其他角色？</a></li> 
<li>此例項中的API使用者為何？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>角色</td> 
   <td><li>有多少角色？</li>  
<li>什麼 <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">許可權/存取</a> 每個角色都有嗎？ 是否應對任何專案進行調整？</li>
<li>每個角色有多少使用者？</li>
<li>使用者頻率 <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">登入</a>？</li>
<li>每個API使用者是否有 <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">擁有的使用者角色</a>？ 如果不能，請考慮實作此專案以更輕鬆進行疑難排解。</li> 
<li>您的使用者角色和許可權是否與公司資料一致 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">隱私權原則</a>？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>內部檔案</td> 
   <td><li>貴組織中是否清楚定義使用者和角色？</li>
<li>您新增使用者/管理員的程式為何？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>沙箱（如果適用）</td> 
   <td><li>您是否有 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙箱執行個體</a>？ 如果是這樣的話，請檢閱上述適用於您的沙箱的類別。</li>
<li>是 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">程式匯入</a> 連結至您的沙箱？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 稽核軌跡 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>稽核軌跡</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">誰在工作</a> 在執行個體中？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 工作區與分割區 {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>工作區與分割區</td> 
   <td><li>您有多少工作區和/或分割區？</li>
<li>每個工作區與分割區的主要用途為何？</li>
<li>他們是否需要稽核或變更？</li>
<li>您的工作區與資料分割之間的關係為何？</li>
<li>每個工作區有多少使用者擁有存取權？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>內部檔案</td> 
   <td><li>如何定義工作區和分割區？</li>
<li>將工作區新增至您的執行個體或將使用者新增至工作區的程式為何？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Smart Campaign {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>Smart Campaign設定</td> 
   <td><li>您是否對Smart Campaign的大小有限制？</li>
<li>如果沒有，請考慮新增一個。 我們建議將智慧行銷活動限制限制限製為資料庫的25%，以避免在工作流程中過度通訊或處理整個資料庫，這不僅可保護您的品牌，還有助於保護執行個體的效能。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 通訊限制 {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>通訊限制</td> 
   <td><li>是否有限制？ 貴企業是否有可能需要通訊限制的原則？</li>
<li>Adobe建議將通訊限製為每天1封，每7天3封，並封鎖非運作電子郵件。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 標記 {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>標記</td> 
   <td><li>標籤數量有多少？ 目前使用多少個標籤？ 是否需要新增？</li>
<li>您的程式是否需要標籤？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>頻道</td> 
   <td><li>有多少管道？ 目前使用多少個？</li>
<li>所有管道計畫狀態是否都適當？ 它們是否在計畫中顯示進度？</li>
<li>您的管道是否與特定計畫型別有關？</li>
<li>每個管道的哪些狀態被視為成功？ 這些是否符合您的行銷目標？</li>
<li>是否正確使用營運管道？</li>
<li>針對進階Report Builder（收入週期總管\RCE），您的管道分析行為是否設定為符合納入期間成本的方案實務？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>行銷行事曆（如果適用）</td> 
   <td><li>有多少行事曆專案型別？ 它們是否仍然相關？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 資料庫管理 {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>欄位管理</td> 
   <td><li>有多少欄位？ 按一下「匯出欄位名稱」以檢閱欄位、自訂欄位及其API名稱的清單。</li>
<li>有多少自訂欄位？</li>
<li>使用了多少欄位？ 在「欄位動作」下拉式清單中選取「匯出使用者」，即可檢閱欄位的相關資產。</li>
<li>Marketo Engage與您的CRM之間同步了多少次？</li>
<li>CRM欄位是否已同步至適當的物件？</li>
<li>有針對人員詳細資料設定的自訂檢視嗎？ 應該有嗎？</li>
<li>根據來源，您的欄位是否有命名慣例？ 如果沒有，請考慮實作此專案。</li>
<li>是否有任何欄位遭到封鎖？ 請務必瞭解原因。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>自訂活動</td> 
   <td><li>是否有任何自訂活動？</li>
<li>若是如此，請按一下這些欄位，瞭解哪些活動與Marketo表單、電子郵件或登入頁面無關。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>自訂物件</td> 
   <td><li>有多少自訂物件？ 他們如何同步至您的CRM？</li>
<li>您的程式和清單查詢如何使用這些自訂物件？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 整合 {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>您正在同步至哪個CRM？ Salesforce? MS Dynamics？ 維耶娃？</li>
<li>自訂同步還是雙向？ （KG：修正文法並檢查重要性）</li>
<li>[僅限Salesforce]您的執行個體是否已實作自訂同步篩選器？ 請聯絡Marketo支援以識別自訂同步篩選器，或要求實作自訂同步規則。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>登陸頁面</td> 
   <td><li>網域設定為何？</li>
<li>後援設定為何？</li>
<li>首頁設定為何？</li>
<li>是否啟用表單預填？</li>
<li>個人化URL已啟用嗎？</li>
<li>有重新導向的規則設定嗎？</li>
<li>您有設定好的網域別名嗎？ 您是否透過檔案追蹤您如何使用網域別名？</li>
<li>是否啟用登入頁面的安全網域？ 確認您的登入頁面資產是否包含「http」URL。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>您的網站是否有Munchkin追蹤程式碼(不在Marketo中)？</li>
<li>是否啟用「不要追蹤」瀏覽器請求？</li>
<li>您的Munchkin API已設定嗎？ 如果您遺失munchkin程式碼在網站上的位置檔案，請在基本的「Analytics」中使用「網頁分析報表」，以快速檢視方式開始瞭解Munchkin程式碼在您網站上的放置位置。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>網站服務</td> 
   <td><li>是否已啟用IP限制？ 他們應該是？</li>
<li>哪些使用者/應用程式正在您的執行個體中進行API呼叫？</li>
<li>您是否達到或接近達到API限制？ 如果是這樣的話，請考慮增加此功能或稽核您的執行個體，以叫停這些API呼叫。</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight （如果適用）</td> 
   <td><li>具有 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">已安裝MSI套件</a>？</li>
<li>有您 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">升級至最新版Sales Insight</a>？</li>
<li>您是否已完成Sales Insight設定？ 企業/無限制使用者 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">按一下這裡</a>，專業使用者 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">按一下這裡</a>.</li>
<li>有您 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">為您的使用者授與存取權</a> 是否根據您購買的座位數？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>啟動點（如果適用）</td> 
   <td><li>您已設定哪些服務（網路研討會、廣告等）？ 是否有任何已接近其有效期的專案？</li>
<li>您的整合使用多少API呼叫？</li>
<li>您是否已為使用案例制定正確的整合？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Webhook （如果適用）</td> 
   <td><li>您已設定哪些連線？</li>
<li>任何已不再使用嗎？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>行動應用程式（如適用）</td> 
   <td><li>您有哪些行動應用程式？</li>
<li>已新增哪些測試裝置？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 寶箱 {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>寶箱</td> 
   <td><li>寶藏箱中開啟了什麼功能？</li>
<li>是否有應開啟或關閉的功能？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>行銷活動檢視窗</td> 
   <td><li>是否已開啟行銷活動稽核檢查？</li>
<li>如果沒有，請考慮將其開啟，以輕鬆識別哪些促銷活動正在作用中、與您的CRM同步，及/或刪除記錄。</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## 其他 {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>Marketo Engage狀態更新</td> 
   <td><li>您的執行個體是否已註冊Marketo Engage狀態更新？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>授權連絡人</td> 
   <td><li>您在支援入口網站中設定適當的授權連絡人了嗎？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>警示</td> 
   <td><li>是否有任何從Marketo Engage傳送給內部團隊的有效警示？</li>
<li>如果有的話，這些警報是否可正常運作？</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>通知</td> 
   <td><li>您訂閱了適當的管理員通知嗎？</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
