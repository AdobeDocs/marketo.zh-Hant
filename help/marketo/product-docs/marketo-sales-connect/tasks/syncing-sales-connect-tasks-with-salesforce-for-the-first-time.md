---
unique-page-id: 14352541
description: 首次將銷售連線工作與Salesforce同步——行銷人員檔案——產品檔案
title: 首次將Sales Connect工作與Salesforce同步
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 首次將Sales Connect工作與Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Connect和Salesforce工作之間的同步時，我們會匯入您的Salesforce工作。 我們不 **會推送** Sales Connect中您目前在Salesforce中的任何工作。 為了減少雜亂和重複，從Sales Connect同步到Salesforce的唯一任務是在Sales Connect與SFDC同步 *後* ，建立的任務。

以下是同步Sales Connect和SFDC任務時的情況：

- 當您按一下「儲存」進行工作同步時，就會開始同步。 這最初需要一些時間。

- 在中更新或建立的任何提醒 `last 24 hours` 都將從SFDC提取到Sales Connect。 同步是基於 `due date` 的，所有這些任務都將在後端同步，但在命令中心，您將只看到今天和明天的任務。

- 如果以前已開啟同步，而您刪除了SFDC中的任何任務，則過去15天內刪除的任何任務都將從命令中心刪除。

- 只要同步處於啟用狀態，我們就會在Sales Connect和SFDC之間不斷同步任務。

在初始同步後，您在Sales Connect中建立、編輯、完成或刪除的任何工作，都會同步至Salesforce中的工作清單。 任何在Salesforce中建立、編輯、完成或刪除的作業，都會在Sales Connect中更新您的工作清單。

若要開啟此同步，只要勾選Web應用程式中「設 [定」頁面中的](http://toutapp.com/next#settings/crm/salesforce/configure) 「同步」方塊。

