---
description: 為您新的Marketo Engage執行個體設定Analytics區段。
title: 新執行個體最佳實務 — 分析檢查清單
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 新執行個體最佳實務：Analytics檢查清單 {#new-instance-best-practices-analytics-checklist}

Analytics區段提供可分析行銷工作績效的全域報表。 瞭解導覽的必要步驟。

記得要[下載檢查清單](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)並追蹤您的進度。

## 樹狀 {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">面積圖</th>
    <th style="width:80%">動作專案</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>組織：命名、資料夾和封存</td>
    <td><li>使用報告命名慣例來區分「全域報告」標籤中的報告。
    <ul><li>良好命名慣例的範例是[Report Type] [Global vs. BU-Specific Tag] [Report Description]，例如[Email Performance]-[Global]-[180 Days Email Engagement]。</li></ul><br>
    <li>識別應與您組織內不同使用者群組（例如銷售團隊、行銷領導力）共用的報告，並在Analytics for Global Reports的「群組報告」資料夾中依資料夾整理報告。</li> 
    <li>封存應限制在全域報告資料夾中，因為這些報告一律開啟。   <ul><li>如果您是根據業務單位結構製作報表，請將封存限製為組織變更，例如減少或新增相關業務單位。</li></ul>
    </td>
  </tr>
  <tr>
    <td>工作區（如果適用）</td>
    <td><li>跨工作區復寫全域報表和資料夾結構，以維持團隊的一致報表。 這些報表會位於「群組報表」資料夾中。</li></td>
  </tr>
  <tr>
    <td>我的報告</td>
    <td><li>識別並建立在<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">我的報告</a>區段中使用的所需報告。 使用此私人報告區段作為全域報告的沙箱。 這些量度僅供建立報表的使用者使用。</li>
    <li>使用您組織的命名慣例來識別報告及使用方式，讓您能夠協調「我的報告」中的報告與「群組報告」中的報告。</li></td>
  </tr>
  <tr>
    <td>群組報表</td>
    <td><li>群組報告是您組織的全域報告，應報告組織的整體活動。</li>
    <li>請考慮建立<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">可複製的核心報表</a>，讓每個業務單位最常使用，以縮短提取報表所需的時間，並確保資料正確無誤。 請參閱下列<a href="#global-reports">全域報告表格的詳細資料</a>。
    <ul><li>依來源、月份的人員績效報表（所有時間且以時間為基礎）</li>
    <li>方案績效報表（依成本月份、以時間為基礎）</li>
    <li>電子郵件效能報表（以時間為基礎）</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">在報表的「設定」標籤中開啟「全域報告」</a>，將您所有工作區的資料加入電子郵件效能和電子郵件連結效能報表。 如果您有多個工作區，則只需在預設工作區中啟用它即可。</li>
    <p><img src="assets/tip-icon.png" alt="附註圖示"> 秘訣：使用您要包含在資料庫區段的大部分報表中的篩選器，建立<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">智慧清單</a>。 當您需要更新智慧列示條件時，可以在一個位置更新它，而不是在所有全域報告中更新。</td>
  </tr>
</tbody>
</table>

## 訂閱 {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">面積圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>訂閱</td>
    <td><li>與行銷主管保持一致，瞭解應檢閱報表結果以及實施期間其順序的人員。</li> <li>使用訂閱將資料散發給組織中的需要瞭解的人，而不用用盡指名的使用者授權。</li>
    <p><img src="assets/tip-icon.png" alt="附註圖示"> 提示：如果您希望使用者存取即時報表資料，您必須將他們新增為使用者，以便他們檢視報表。
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">以所需的節奏（每日/每週/每月）設定訂閱</a>，以供每個團隊持續監控。 您也可以<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">在Analytics的「訂閱」標籤下方的同一位置，檢視您的所有訂閱</a>。</li></td>
  </tr>
</tbody>
</table>

## 全域報告 {#global-reports}

識別應與您組織內不同使用者群組（例如銷售團隊、行銷領導力）共用的報表。 為每個團隊/使用者群組/業務單位建立適當的檔案夾結構，以便在「群組報表」中組織複製報表。 請考慮設定全域報表，例如：

<table>
<thead>
  <tr>
    <th style="width:20%">報告型別</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>以電子郵件傳送效能報表</td>
    <td><li>使用選取的正確電子郵件建立全域、Workspace/業務單位報告。</li>
    <li>在所有可複製的計畫範本中建立本機電子郵件效能報告。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">使用相關的時間範圍</a> （例如YTD、過去90天等） 報表，以提供標準電子郵件參與度和傳遞能力量度的精確檢視。</li>
    <p><img src="assets/tip-icon.png" alt="附註圖示"> 提示： <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">在<strong>管理員&gt;電子郵件</strong></a>中開啟「機器人活動」篩選以避免記錄，或識別是否針對機器人活動啟用記錄。 包含篩選器，僅允許在可複製全域報告的智慧清單中<a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">開啟/點選的活動，「是機器人活動」限製為「False」</a>。</td>
  </tr>
  <tr>
    <td>人員績效報表</td>
    <td><img src="assets/note-icon.png" alt="附註圖示"> 注意：建議您為每個Marketo Engage實作設定適當的<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">管道和標籤策略</a>，才能依管道追蹤已獲得的人員以及行銷投資的ROI。
    <p>
    <li>決定您將用來測量潛在客戶贏取計畫績效的標準，並根據這些量度建立以時間為基礎的標準報表（今年度、最近滾動的12個月檢視或180天）： <ul><li>贏取方案：為取得人員而記入點數的Marketo Engage方案。</li>
    <li>人員Source：資料庫得知記錄的來源類別（根據CRM中的來源值清單）
    </li></ul>
    <li>按周或月建立測量人員。 此報告可提供資料庫成長率的測量值，以及您是否接近資料庫大小限制。</li>
    <li>使用您的智慧列示作為自訂欄，依<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">篩選「人員效能報表」中的量度。</a></li>
    <p><img src="assets/tip-icon.png" alt="附註圖示"> 提示：為您要新增至資料庫中「人員績效報表」的自訂欄（而非「行銷活動」）建立「智慧列示」，以便在報表中選取「智慧列示」名稱時，能夠正確且清楚地看到該名稱。</td>
  </tr>
  <tr>
    <td>程式效能報表</td>
    <td><p><img src="assets/note-icon.png" alt="附註圖示"> 注意：此報表要求您在<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>管理員</strong> &gt; <strong>標籤</strong></a>中定義管道、進度狀態和成功步驟。
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">在選擇性方案中測量行銷策略的有效性</a>。</li>
    <li>根據行銷活動中的最佳實務管理方案會籍（使用Smart Campaigns更新贏取方案、狀態、成功狀態）。</li>
    <li>根據本年度與累計12個月的成本進行測量。
    <ul><li>請記住，維護<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">期間成本</a>對於運用方案績效報表至關重要。</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="附註圖示">秘訣：若要彙總並檢視方案績效報表中的任何<a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">匯入清單</a>，請確定您的團隊選取適當的贏取方案以進行標籤。 當匯入的清單不適用於任何管道時，請考慮建立<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">要選取作為贏取程式的預設程式</a>。 這可確保任何匯入的人員擁有與來源、業務單位、管道等相關的有效贏取計畫，而不是空白值。</td>
  </tr>
  <tr>
    <td>登陸頁面效能報表</td>
    <td><li>將<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">登陸頁面效能報表</a>建立為全域報表，讓您可以在一個位置<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">篩選及檢閱您所有設計工作室/行銷活動登陸頁面的數量</a>。</li>
    <li>對於具有登入頁面的程式，請考慮在程式範本中<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">建立專屬的本機報告</a>，以便在程式層級檢閱效能。</li></td>
  </tr>
  <tr>
    <td>網頁活動報表</td>
    <td><img src="assets/note-icon.png" alt="附註圖示"> 注意：在此報表中只會追蹤已啟用<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a>的網頁(外部和Marketo登陸頁面)。 請考慮將JavaScript程式碼放在Tag Management平台中(例如<a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>)，以避免在每個網頁上以硬式編碼撰寫程式碼。
    <p>
    <li>將<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">網頁活動報告</a>建立為全域報告，以便您可以集中檢閱所有網頁的數字。 請注意，您的外部網頁活動只會反映在網頁活動報表中。</li></td>
  </tr>
</tbody>
</table>

## 本機報表 {#local-reports}

有些Marketo Engage報表最適合部署為行銷活動特定方案中的本機資產，因為這類報表的一般用途是一組較有限的方案和資產。 請考慮設定基本報表，例如：

<table>
<thead>
  <tr>
    <th style="width:20%">報告型別</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>以電子郵件傳送連結效能報表</td>
    <td><li>在傳送電子郵件的程式和您的滴答式行銷活動中建立<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">電子郵件連結效能報表</a>，以提供您電子郵件傳送中人們點按之連結的深入分析。</li></td>
  </tr>
  <tr>
    <td>行銷活動報表</td>
    <td><li>建立<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">行銷活動報告</a>，並在行銷活動的作業資料夾中選擇一個期間。</li>
    <li>設定報告以監視每個使用案例的觸發程式，並<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">套用促銷活動篩選器</a> （例如，行為評分觸發程式、生命週期資格觸發程式、興趣時刻觸發程式）。</li></td>
  </tr>
  <tr>
    <td>參與資料流績效報表（如果適用）</td>
    <td><li>建立<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">參與資料流績效報表</a>，以評估在參與方案中部署的內容和資料流的成效。</li>
    <li>請考慮在報告的「設定」標籤</a>中使用<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">「分段」篩選器，並依照參與計畫中使用的<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">區段</a> （例如，人員來源、產業）來分組報告資料。 這有助於深入瞭解每個區段的參與模式，引導您進行策略變更以改進參與計畫（內容、串流、串流順序等）。</li></td>
  </tr>
</tbody>
</table>
