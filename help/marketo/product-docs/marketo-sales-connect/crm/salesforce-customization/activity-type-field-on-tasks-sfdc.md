---
unique-page-id: 14352476
description: 任務活動類型欄位(SFDC)-行銷文檔——產品文檔
title: 任務上的活動類型欄位(SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 任務(SFDC){#activity-type-field-on-tasks-sfdc}上的活動類型欄位

在Sales Connect的協助下，您可以將電子郵件和呼叫記錄為Salesforce中的活動。 在Salesforce中擁有重要資料的關鍵部分，是讓「類型」欄位填入正確值。

>[!NOTE]
>
>透過密件副本記錄電子郵件時，不會查看「任務類型」選取清單，而會自動將類型欄位填入為「電子郵件」，因為這些電子郵件會透過密件副本位址傳送至Salesforce。

## 要求{#requirements}

* 與Salesforce的連線
* 未在「任務類型」選擇清單中選擇預設類型值
* 「呼叫」、「回覆」和「電子郵件」必須都存在於「任務類型」選取清單下（大寫事項）
* 沒有工作流或觸發器對「類型」欄位的值執行操作

## 設定{#setup}

首先檢查您是否有正確的挑選清單值。 您將需要Salesforce管理員的協助，才能變更您的選取清單。

1. 導覽至[Salesforce.com](https://salesforce.com)，然後按一下右上角的「設定」。
1. 按一下「自訂」。
1. 按一下「活動」。
1. 按一下「工作欄位」。
1. 按一下「類型」。
1. 您現在位於「任務類型選擇清單」中。 請確定未選取「預設」。
1. 請確定「電子郵件」、「呼叫」和「回覆」的「類型」值已列出。

現在，您會開始看到「類型」欄位填入已記錄之「電子郵件」、「呼叫」和「回覆」的對應值。 這些值將&#x200B;**not**&#x200B;填入Sales Connect提醒任務。

>[!NOTE]
>
>如果您未將&#39;Reply&#39;視為值，請按一下&#x200B;**New**&#x200B;加入。 「回覆」不是Salesforce中的標準值。
