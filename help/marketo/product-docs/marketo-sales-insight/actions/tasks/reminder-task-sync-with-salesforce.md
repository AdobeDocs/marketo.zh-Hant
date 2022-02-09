---
description: 提醒任務與Salesforce同步 — Marketo文檔 — 產品文檔
title: 提醒任務與Salesforce同步
hide: true
hidefromtoc: true
source-git-commit: acb077e9d6e9fa4027d660ee182a13820f16ad83
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 提醒任務與Salesforce同步 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>瞭解如何啟用任務同步簽出 [將Sales Insight操作任務/提醒同步到Salesforce任務](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks)。

啟用任務同步設定後，用戶將看到其提醒任務與Salesforce雙向同步。 這意味著用戶可以從Salesforce或Sales Insight Actions管理任務，並確信系統將保持一致。

## 提醒任務欄位同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

下面是Sales Insight Actions中的提醒任務欄位及其相應的Salesforce欄位的清單，這些欄位通過雙向任務同步受支援。

<table>
 <tr>
  <th>Sales Insight活動任務欄位</th>
  <th>Salesforce任務欄位</th>
  <th>Salesforce任務</th>
 </tr>
 <tr>
  <td>任務名稱</td>
  <td>主題欄位</td>
  <td>一個短摘要欄位，用於顯示任務的標題。</td>
 </tr>
 <tr>
  <td>狀態</td>
  <td>任務狀態</td>
  <td><p>顯示任務的狀態。 Sales Insight Actions任務有兩個狀態，它們映射到Salesforce任務狀態選擇清單中的兩個值。</p>
  <p>在Sales Insight Actions中開啟=未在Salesforce中啟動。</p>
  <p>在Sales Insight活動中完成=在Salesforce中完成。</p>
  <p>Salesforce中的其他狀態值將不會同步到Sales Insight Actions。</p></td>
 </tr>
 <tr>
  <td>優先順序</td>
  <td>優先順序</td>
  <td><p>Sales Insight Actions優先順序可以是「正常」或「高」，它映射到Salesforce中的「正常」和高優先順序值。</p>
  <p>Salesforce中的低優先順序值將不會同步到Sales Insight Actions。</p></td>
 </tr>
 <tr>
  <td>到期日</td>
  <td>到期日</td>
  <td>任務到期的日期。</td>
 </tr>
 <tr>
  <td>詳細資訊</td>
  <td>注釋</td>
  <td>顯示有關應使用提醒任務完成的內容的詳細資訊。</td>
 </tr>
</table>

## 首次將Sales Insight Actions任務與Salesforce同步 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

當您首次啟用Sales Insight Actions和Salesforce任務之間的同步時，我們將導入您的Salesforce任務。 我們會 **不** 將您在Sales Insight Actions中擁有的任何當前任務推送到Salesforce。 為減少雜亂和重複，從Sales Insight Actions同步到Salesforce的任務只有建立 *後* 將Sales Insight Actions與SFDC同步。

以下是同步Sales Insight Actions和SFDC任務時發生的情況：

* 一旦按一下「保存任務」同步，它們就開始同步。 這需要一些時間。

* 在過去24小時內更新或建立的任何提醒都將從SFDC拉入到Sales Insight Actions。 同步基於到期日期，所有這些任務都將在後端進行同步，但在命令中心中，您將只看到今天和明天到期的任務。

* 如果以前已啟用同步並且您刪除了SFDC中的任何任務，則在過去15天內刪除的任何任務都將從命令中心刪除。

* 只要啟用同步，我們就會在Sales Insight Actions和SFDC之間不斷同步任務。

在初始同步後，您在Sales Insight Actions中建立、編輯、完成或刪除的任何任務都將同步到Salesforce中的任務清單。 任何在Salesforce中建立、編輯、完成或刪除的內容都將更新Sales Insight Actions中的任務清單。

要開啟此同步，請選中 [「設定」頁](https://toutapp.com/login) 的子菜單。

>[!NOTE]
>
>任務的主題欄位可以在Sales Insight Actions中更新，如果您正在使用 `{{activity_subject}}` 動態欄位 [活動詳細資訊自定義](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 的子菜單。 相反，對Salesforce中主題欄位所做的任何更新都將 _不_ 同步到Sales Insight Actions提醒任務主題欄位。
