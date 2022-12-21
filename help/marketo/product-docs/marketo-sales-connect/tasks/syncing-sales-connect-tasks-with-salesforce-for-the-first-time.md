---
unique-page-id: 14352541
description: 首次將銷售連線任務與Salesforce同步 — Marketo檔案 — 產品檔案
title: 首次將銷售連接任務與Salesforce同步
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 首次將銷售連接任務與Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Connect和Salesforce任務之間的同步時，我們將導入您的Salesforce任務。 我們會 **not** 將Sales Connect中的任何當前任務推送到Salesforce。 為了減少雜亂和重複，從Sales Connect同步到Salesforce的任務只有建立的任務 *after* 您將Sales Connect與SFDC同步。

以下是同步Sales Connect和SFDC任務時會發生的情況：

- 當您按一下「儲存」時，即會開始同步工作。 這需要一些時間。

- 在過去24小時內更新或建立的任何提醒都將從SFDC提取到Sales Connect。 同步基於到期日，所有這些任務都將在後端同步，但在命令中心，您將只看到今天和明天的任務。

- 如果以前已開啟同步，而您刪除了SFDC中的任何任務，則在過去15天中被刪除的任何任務都將從命令中心中刪除。

- 只要啟用同步，我們就會在Sales Connect和SFDC之間不斷同步任務。

初始同步後，您在Sales Connect中建立、編輯、完成或刪除的任何任務都將同步到Salesforce中的任務清單。 而任何在Salesforce中建立、編輯、完成或刪除的內容都將在Sales Connect中更新您的任務清單。

若要開啟此同步，只要勾選 [設定頁面](https://toutapp.com/login) 在web應用程式中。
