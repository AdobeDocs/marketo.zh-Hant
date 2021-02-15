---
unique-page-id: 14352541
description: 首次將銷售連線工作與Salesforce同步——行銷人員檔案——產品檔案
title: 首次將Sales Connect工作與Salesforce同步
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 首次將Sales Connect Tasks與Salesforce同步{#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Connect和Salesforce工作之間的同步時，我們會匯入您的Salesforce工作。 我們將&#x200B;**not**&#x200B;推送您在Sales Connect到Salesforce中的任何目前工作。 為了減少雜亂和重複，從Sales Connect到Salesforce中同步的唯一任務是在&#x200B;*將Sales Connect與SFDC同步後建立的*&#x200B;任務。

以下是同步Sales Connect和SFDC任務時的情況：

- 當您按一下「儲存」進行工作同步時，就會開始同步。 這最初需要一些時間。

- 在過去24小時內更新或建立的任何提醒都將從SFDC提取到Sales Connect。 同步是基於到期日，所有這些任務都將在後端同步，但在命令中心中，您將只看到今天和明天的任務。

- 如果以前已開啟同步，而您刪除了SFDC中的任何任務，則過去15天內刪除的任何任務都將從命令中心刪除。

- 只要同步處於啟用狀態，我們就會在Sales Connect和SFDC之間不斷同步任務。

在初始同步後，您在Sales Connect中建立、編輯、完成或刪除的任何工作，都會同步至Salesforce中的工作清單。 任何在Salesforce中建立、編輯、完成或刪除的作業，都會在Sales Connect中更新您的工作清單。

若要開啟此同步，只要勾選Web應用程式中[設定頁面](https://toutapp.com/login)的同步方塊即可。
