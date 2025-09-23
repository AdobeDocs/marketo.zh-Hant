---
unique-page-id: 14352541
description: 首次將Sales Connect工作與Salesforce同步 — Marketo檔案 — 產品檔案
title: 首次將 Sales Connect 工作與 Salesforce 同步
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 3%

---

# 第一次將[!DNL Sales Connect]個任務與[!DNL Salesforce]同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟[!DNL Sales Connect]與[!DNL Salesforce]個任務之間的同步時，我們會匯入您的[!DNL Salesforce]個任務。 我們&#x200B;**不會**&#x200B;將您在[!DNL Sales Connect]中擁有的任何目前任務推播到[!DNL Salesforce]。 若要減少雜訊和重複專案，從[!DNL Sales Connect]同步到[!DNL Salesforce]的唯一工作是在您將&#x200B;*與SFDC同步*&#x200B;後[!DNL Sales Connect]建立的工作。

以下是當您同步[!DNL Sales Connect]和SFDC任務時發生的情況：

- 當您在同步處理任務時按一下「儲存」，任務就會開始進行同步處理。 這最初需要一些時間。

- 任何在過去24小時內已更新或建立的提醒將會從SFDC提取至[!DNL Sales Connect]。 同步是以到期日為基礎，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天到期的工作。

- 如果先前已開啟同步功能，而您又刪除了SFDC中的任何工作，則任何過去15天中刪除的工作都會從命令中心刪除。

- 只要同步處理已啟用，我們就會持續在[!DNL Sales Connect]和SFDC之間同步處理工作。

初次同步之後，您在[!DNL Sales Connect]中建立、編輯、完成或刪除的任何工作都會同步至[!DNL Salesforce]中的工作清單。 在[!DNL Salesforce]中建立、編輯、完成或刪除的任何專案都會在[!DNL Sales Connect]中更新您的任務清單。

若要開啟此同步，只要在Web應用程式的[設定頁面](https://toutapp.com/login)中勾選同步方塊即可。
