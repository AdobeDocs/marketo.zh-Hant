---
unique-page-id: 14352541
description: 首次將Sales Connect工作與Salesforce同步 — Marketo檔案 — 產品檔案
title: 首次將Sales Connect工作與Salesforce同步
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 首次將Sales Connect工作與Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Connect與Salesforce工作之間的同步時，我們會匯入您的Salesforce工作。 我們會 **非** 將您在Sales Connect中擁有的任何目前工作推播到Salesforce。 為了減少雜湊和重複專案，從Sales Connect同步至Salesforce的唯一工作就是建立的工作 *晚於* 您將Sales Connect與SFDC同步。

以下是同步處理Sales Connect與SFDC工作時所發生的情況：

- 當您在同步處理任務時按一下「儲存」，任務就會開始進行同步處理。 這最初需要一些時間。

- 過去24小時內已更新或建立的任何提醒都會從SFDC提取至Sales Connect。 同步是以到期日為基礎，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天到期的工作。

- 如果先前已開啟同步，而您刪除了SFDC中的任何工作，則過去15天刪除的任何工作都會從指揮中心刪除。

- 只要已啟用同步處理，我們就會持續在Sales Connect與SFDC之間同步處理工作。

初次同步後，您在Sales Connect中建立、編輯、完成或刪除的任何工作都會同步至Salesforce中的工作清單。 在Salesforce中建立、編輯、完成或刪除的任何專案，都會在Sales Connect中更新您的工作清單。

若要開啟此同步，只要勾選您電腦中的同步方塊即可 [設定頁面](https://toutapp.com/login) 在網頁應用程式中。
