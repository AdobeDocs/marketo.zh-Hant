---
description: 記錄新Marketo Engage執行個體的設定。
title: 新執行個體最佳實務 — 記錄您的設定
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
TQID: https://experienceleague.adobe.com/pqbf84tAUt49rWUD7rONRuZNgR8v5yMmYTqwqlXqgAs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 536
ht-degree: 4%

---

# 新執行個體最佳做法：記錄您的設定 {#new-instance-best-practices-document-your-setup}

現在您已瞭解為新的Marketo Engage執行個體設定所需的主要產品領域，下一步是建立執行個體設定和技術棧疊的檔案。 不論您是透過試算表或專案管理應用程式建立例項，您的檔案都是追蹤進度和記錄詳細資料的絕佳資源，也能讓您的例項結構化，並可持續供組織內的未來行銷人員使用。

## 資料 {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>清單匯入</td>
    <td><li>收集資料來源清單，這些記錄將從這裡提取到<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">匯入Marketo Engage</a>。</li>
    <li>如果您要從多個資料來源匯入，請考慮使用主清單或在人員記錄上建立<a href="https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">自訂欄位</a>來表示資料來源。</li></td>
  </tr>
  <tr>
    <td>資料庫整合</td>
    <td><li>如果利用Marketo Engage與您的CRM之間的原生同步，請仔細考慮您要在系統之間同步的欄位。 並非每個欄位都需要同步，因此請對資料流程保持策略性。</li></td>
  </tr>
</tbody>
</table>

## 文件 {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">區域圖</th>
    <th style="width:80%">動作專案</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>使用者</td>
    <td><li>基於安全理由，記錄您執行個體中的<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">目前使用者</a>。 以下詳細資料應至少包含在內（前往「管理員&gt;使用者和角色」即可全部看到）：</li>
    <ul>
    <li>名稱</li>
    <li>電子郵件</li>
    <li>登入</li>
    <li>角色</li>
    <li>存取權到期日</li>
    <li>使用者建立日期</li>
    <li>最近登入日期</li></ul>
    <p><img src="assets/note-icon.png" alt="附註圖示"> 注意：您也可以展開此專案，加入角色/許可權的相關檔案。
    <p>
    <li>身為Marketo Engage產品管理員，需開發內部流程，以定期稽核及更新Marketo Engage使用者清單。 若要變更Adobe Admin Console中的使用者清單，請考慮<a href="https://helpx.adobe.com/tw/enterprise/using/users.html" target="_blank">大量動作</a>，例如上傳.CSV、使用「使用者管理REST API」等</li></td>
  </tr>
  <tr>
    <td>組織</td>
    <td><li>記錄協定的資料夾結構、方案、資產等的標準命名慣例，以及做出決定背後的原因。 <a href="https://experienceleague.adobe.com/zh-hant/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">在這裡進一步瞭解最佳實務。</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>建立變更記錄檔，您可以在其中記錄執行個體中的變更專案以及修改的原因。 <a href="https://experienceleague.adobe.com/zh-hant/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">在這裡進一步瞭解最佳實務。</a></li></td>
  </tr>
  <tr>
    <td>教戰手冊</td>
    <td><li>為內部使用者加入執行個體建立使用者教戰手冊或管理教戰手冊。</li></td>
  </tr>
  <tr>
    <td>與內部團隊的交談</td>
    <td><li>讓內部行銷團隊的Marketo Engage期望與Marketo Engage的功能保持一致。</li>
    <li>確定在Marketo Engage例項中將成為您利害關係人的團隊，並記錄他們使用Marketo Engage作為技術要實現的目標。</li></td>
  </tr>
  <tr>
    <td>工作區與分割區（如果適用）</td>
    <td><li>記錄工作區的定義方式以及與資料庫分割相關的方式（例如，顯示每個人相對於業務部門的全域工作區）。</li>
    <li>將新記錄匯入適當的資料分割。</li>
    <li>在您的CRM中定義值，該值會將使用者放置在適當的資料分割中。</li></td>
  </tr>
</tbody>
</table>
