---
description: 與Salesforce同步的提醒任務 — Marketo檔案 — 產品檔案
title: 與Salesforce的提醒任務同步
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 與Salesforce的提醒任務同步 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>了解如何啟用任務同步簽出 [同步Sales Insight操作任務/提醒至Salesforce任務](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

啟用任務同步設定後，用戶將看到其提醒任務與Salesforce雙向同步。 這表示使用者可以從Salesforce或Sales Insight Actions管理任務，並確信系統會保持一致。

## 提醒任務欄位同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

下面是Sales Insight Actions中的提醒任務欄位清單，以及通過雙向任務同步支援的相應Salesforce欄位。

<table>
 <tr>
  <th>Sales Insight Actions任務欄位</th>
  <th>Salesforce任務欄位</th>
  <th>Salesforce任務</th>
 </tr>
 <tr>
  <td>任務名稱</td>
  <td>主旨欄位</td>
  <td>一個短摘要欄位，用於顯示任務的標題。</td>
 </tr>
 <tr>
  <td>狀態</td>
  <td>任務狀態</td>
  <td><p>顯示任務的狀態。 Sales Insight Actions任務有兩種狀態，它們對應到Salesforce任務狀態選擇清單中的兩個值。</p>
  <p>在Sales Insight Actions中開啟= Salesforce中未開始。</p>
  <p>Sales Insight Actions中的Complete = Salesforce中的Completed。</p>
  <p>Salesforce中的其他狀態值將不會同步至Sales Insight Actions。</p></td>
 </tr>
 <tr>
  <td>優先順序</td>
  <td>優先順序</td>
  <td><p>Sales Insight Actions優先順序可以是「正常」或「高」，它映射到Salesforce中的「正常」和「高」優先順序值。</p>
  <p>Salesforce中的低優先順序值將不會同步至Sales Insight Actions。</p></td>
 </tr>
 <tr>
  <td>到期日</td>
  <td>到期日</td>
  <td>任務到期的日期。</td>
 </tr>
 <tr>
  <td>詳細資料</td>
  <td>註解</td>
  <td>顯示有關預定要使用提醒任務完成的內容的詳細資訊。</td>
 </tr>
</table>

## 首次將Sales Insight活動任務與Salesforce同步 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Insight Actions和Salesforce任務之間的同步時，我們會導入您的Salesforce任務。 我們會 **not** 將Sales Insight Actions中的任何當前任務推送到Salesforce。 為了減少雜亂和重複項，從Sales Insight Actions同步到Salesforce中的任務只有建立的任務 *after* 您將Sales Insight Actions與SFDC同步。

以下是同步Sales Insight Actions和SFDC任務時會發生的情況：

* 當您按一下「儲存」時，即會開始同步工作。 這需要一些時間。

* 在過去24小時內更新或建立的任何提醒都將從SFDC提取到Sales Insight Actions。 同步基於到期日，所有這些任務都將在後端同步，但在命令中心，您將只看到今天和明天的任務。

* 如果以前已開啟同步，而您刪除了SFDC中的任何任務，則在過去15天中被刪除的任何任務都將從命令中心中刪除。

* 只要啟用同步，我們就會在Sales Insight Actions和SFDC之間不斷同步任務。

初始同步後，您在Sales Insight Actions中建立、編輯、完成或刪除的任何任務都將同步到Salesforce中的任務清單。 而任何在Salesforce中建立、編輯、完成或刪除的項目，都會在Sales Insight Actions中更新您的任務清單。

若要開啟此同步，只要勾選 [設定頁面](https://toutapp.com/login) 在web應用程式中。

>[!NOTE]
>
>任務的主題欄位可在「銷售分析操作」中更新，並且該更新將在相應同步任務的Salesforce主題欄位中同步(如果您使用 `{{activity_subject}}` 您的 [活動詳細資訊自訂](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 設定。 反之，對Salesforce中的主題欄位所做的任何更新都將 _not_ 同步到「銷售分析活動提醒」任務主題欄位。
