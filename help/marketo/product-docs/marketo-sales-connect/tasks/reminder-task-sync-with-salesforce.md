---
description: 提醒任務與Salesforce同步 — Marketo檔案 — 產品檔案
title: 提醒任務與Salesforce同步
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 提醒任務與Salesforce同步 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>若要瞭解如何啟用「工作同步處理」簽出 [將Sales Connect工作/提醒同步至Salesforce工作](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

啟用工作同步設定後，使用者會看到他們的提醒工作與Salesforce雙向同步。 這表示使用者可以從Salesforce或Sales Connect管理工作，並相信系統會維持一致。

## 提醒工作列位同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下是Sales Connect中的提醒工作欄位清單，以及透過雙向工作同步支援的對應Salesforce欄位。

<table>
 <tr>
  <th>Sales Connect工作欄位</th>
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
  <td><p>顯示工作的狀態。 Sales Connect工作有兩個狀態，對應至Salesforce工作狀態選擇清單中的兩個值。</p>
  <p>在Sales Connect中開啟=未在Salesforce中啟動。</p>
  <p>在Sales Connect中完成=在Salesforce中完成。</p>
  <p>Salesforce中的其他狀態值將不會同步至Sales Connect。</p></td>
 </tr>
 <tr>
  <td>優先順序</td>
  <td>優先順序</td>
  <td><p>Sales Connect優先順序可以是「一般」或「高」，對應至Salesforce中的「一般」和「高」優先順序值。</p>
  <p>Salesforce中的低優先順序值將不會同步至Sales Connect。</p></td>
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

## 首次將Sales Connect工作與Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Connect與Salesforce工作之間的同步時，我們會匯入您的Salesforce工作。 我們會 **非** 將您在Sales Connect中擁有的任何目前工作推播到Salesforce。 為了減少雜湊和重複專案，從Sales Connect同步至Salesforce的唯一工作就是建立的工作 *晚於* 您將Sales Connect與SFDC同步。

以下是同步處理Sales Connect與SFDC工作時所發生的情況：

* 當您在同步處理任務時按一下「儲存」，任務就會開始進行同步處理。 這最初需要一些時間。

* 過去24小時內已更新或建立的任何提醒都會從SFDC提取至Sales Connect。 同步是以到期日為基礎，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天到期的工作。

* 如果先前已開啟同步，而您刪除了SFDC中的任何工作，則過去15天刪除的任何工作都會從指揮中心刪除。

* 只要已啟用同步處理，我們就會持續在Sales Connect與SFDC之間同步處理工作。

初次同步後，您在Sales Connect中建立、編輯、完成或刪除的任何工作都會同步至Salesforce中的工作清單。 在Salesforce中建立、編輯、完成或刪除的任何專案，都會在Sales Connect中更新您的工作清單。

若要開啟此同步，只要勾選您電腦中的同步方塊即可 [設定頁面](https://toutapp.com/login) 在網頁應用程式中。

>[!NOTE]
>
>若您使用「 」，則可在Sales Connect中更新任務的主旨欄位，且此更新會同步至對應同步任務的Salesforce主旨欄位。 `{{activity_subject}}` 您的中的動態欄位 [活動詳細資料自訂](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 設定。 相反地，對Salesforce中的主旨欄位所做的任何更新都將 _非_ 同步至Sales Connect提醒工作主旨欄位。
