---
description: 繼承檔案1 - Marketo檔案 — 產品檔案
title: 繼承檔案1
hide: true
hidefromtoc: true
source-git-commit: 93be928e540fd50d92bef4ead3ea23519de18cce
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 6%

---

# 繼承檔案1 {#inherit-doc-1}

稽核繼承的執行個體看起來可能像是

您是否從其他管理員繼承了現有的Marketo Engage執行個體？ 若是如此，本文會為您提供。

>[!TIP]
>
>如果您是新的Marketo Engage使用者，且不熟悉許多術語，請檢視 [Marketo字彙表](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## 使用者和角色 {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>區域</th> 
   <th>評論焦點</th>
   <th>欄目3</th>
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td><li>有多少使用者？</li>
<li>是否有任何應過期的使用者？</li>
<li>貴公司是否有刪除使用者的相關政策？</li> 
<li>有多少使用者擁有管理員許可權？</li>
<li>這些使用者中的任何一個是否應變更為其他角色？</li> 
<li>此例項中的API使用者為何？</li></td>
   <td>3.1</td>
  </tr>
  <tr> 
   <td>角色</td> 
   <td><li>有多少角色？</li>  
<li>每個角色具有哪些許可權/存取權？ 是否應對任何專案進行調整？</li>
<li>每個角色有多少使用者？</li>
<li>使用者登入的頻率為何？</li>
<li>每個API使用者都有自己的使用者角色嗎？ 如果不能，請考慮實作此專案以更輕鬆進行疑難排解。</li> 
<li>您的使用者角色和許可權是否與公司資料隱私權政策一致？</li></td>
   <td>3.2</td>
  </tr>
  <tr> 
   <td>內部檔案</td> 
   <td><li>貴組織中是否清楚定義使用者和角色？</li>
<li>您新增使用者/管理員的程式為何？</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>沙箱（如果適用）</td> 
   <td><li>您有沙箱執行個體嗎？ 如果是這樣的話，請檢閱上述適用於您的沙箱的類別。</li>
<li>計畫匯入是否與您的沙箱連結？</li></td>
   <td>3.4</td>
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
   <td><li>誰在執行個體中工作？</li></td>
   <td>3.1</td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight （如果適用）</td> 
   <td><li>具有 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">已安裝MSI套件</a>？</li>
<li>有您 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">升級至最新版Sales Insight</a>？</li>
<li>您是否已完成Sales Insight設定？</li>
<li>有您 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">為您的使用者授與存取權</a> 是否根據您購買的座位數？</li></td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
