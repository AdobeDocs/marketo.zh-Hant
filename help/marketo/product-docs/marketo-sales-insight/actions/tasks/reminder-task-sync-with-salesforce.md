---
description: 提醒任務與Salesforce同步 — Marketo檔案 — 產品檔案
title: 提醒任務與Salesforce同步
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 提醒任務與Salesforce同步 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>若要瞭解如何啟用「工作同步處理」簽出 [將Sales Insight動作任務/提醒同步至Salesforce任務](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

啟用工作同步設定後，使用者會看到他們的提醒工作與Salesforce雙向同步。 這表示使用者可以從Salesforce或Sales Insight Actions管理任務，並確信系統將會保持一致。

## 提醒工作列位同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下是「銷售分析動作」中的提醒工作欄位清單，以及透過雙向工作同步支援的對應Salesforce欄位。

<table>
 <tr>
  <th>銷售分析動作工作列位</th>
  <th>Salesforce工作欄位</th>
  <th>Salesforce工作</th>
 </tr>
 <tr>
  <td>任務名稱</td>
  <td>主題欄位</td>
  <td>旨在顯示任務標題的簡短摘要欄位。</td>
 </tr>
 <tr>
  <td>狀態</td>
  <td>任務狀態</td>
  <td><p>顯示工作的狀態。 Sales Insight Actions工作有兩個狀態，對應至Salesforce工作狀態選擇清單中的兩個值。</p>
  <p>在Sales Insight中開啟=未在Salesforce中啟動。</p>
  <p>在Sales Insight中完成=在Salesforce中完成。</p>
  <p>Salesforce中的其他狀態值將不會同步至Sales Insight動作。</p></td>
 </tr>
 <tr>
  <td>優先順序</td>
  <td>優先順序</td>
  <td><p>「銷售分析動作」優先順序可以是「一般」或「高」，對應至Salesforce中的「一般」和「高」優先順序值。</p>
  <p>Salesforce中的低優先順序值不會同步至Sales Insight動作。</p></td>
 </tr>
 <tr>
  <td>到期日期</td>
  <td>到期日期</td>
  <td>任務的到期日。</td>
 </tr>
 <tr>
  <td>詳細資料</td>
  <td>註解</td>
  <td>顯示有關應該完成提醒工作的詳細資訊。</td>
 </tr>
</table>

## 首次與Salesforce同步銷售分析動作工作 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Insight Actions與Salesforce工作之間的同步時，我們會匯入您的Salesforce工作。 我們會 **非** 將您在Sales Insight Actions中擁有的任何目前任務移至Salesforce。 為了減少雜湊和重複專案，從Sales Insight Actions同步至Salesforce的唯一工作就是建立的工作 *晚於* 您可以將Sales Insight動作與SFDC同步。

以下是同步處理Sales Insight動作和SFDC工作時所發生的情況：

* 當您在同步處理任務時按一下「儲存」，任務就會開始進行同步處理。 這最初需要一些時間。

* 過去24小時內已更新或建立的任何提醒都會從SFDC提取至Sales Insight Actions。 同步是以到期日為基礎，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天到期的工作。

* 如果先前已開啟同步，而您刪除了SFDC中的任何工作，則過去15天刪除的任何工作都會從指揮中心刪除。

* 只要同步功能已啟用，我們就會持續在Sales Insight Actions與SFDC之間同步工作。

初次同步後，您在Sales Insight Actions中建立、編輯、完成或刪除的任何工作都會同步至Salesforce中的工作清單。 在Salesforce中建立、編輯、完成或刪除的任何專案，都會更新Sales Insight Actions中的任務清單。

若要開啟此同步，只要勾選您電腦中的同步方塊即可 [設定頁面](https://toutapp.com/login) 在網頁應用程式中。

>[!NOTE]
>
>若您使用「 」，則可在「銷售分析動作」中更新任務的主旨欄位，且此更新會同步至對應同步任務的「銷售人員」主旨欄位。 `{{activity_subject}}` 您的中的動態欄位 [活動詳細資料自訂](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 設定。 相反地，對Salesforce中的主旨欄位所做的任何更新都將 _非_ 同步至「銷售分析動作」提醒任務主旨欄位。
