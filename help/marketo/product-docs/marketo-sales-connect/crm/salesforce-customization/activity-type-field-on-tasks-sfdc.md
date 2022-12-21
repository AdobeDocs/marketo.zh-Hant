---
unique-page-id: 14352476
description: 任務的活動類型欄位(SFDC)- Marketo檔案 — 產品檔案
title: 任務上的活動類型欄位(SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 任務上的活動類型欄位(SFDC) {#activity-type-field-on-tasks-sfdc}

在Sales Connect的協助下，您的電子郵件和呼叫可以記錄為Salesforce中的活動。 在Salesforce中有價值資料的一個關鍵部分是讓「類型」欄位填入正確的值。

>[!NOTE]
>
>透過BCC記錄電子郵件將不會查看「任務類型」選取清單，而是會自動將類型欄位填入為「電子郵件」，因為這些欄位是透過您的BCC地址傳送至Salesforce。

## 需求 {#requirements}

* 與Salesforce的連接
* 未在任務類型選擇清單中選擇預設類型值
* 「任務類型」選擇清單（大寫事項）下必須存在「呼叫」、「回復」和「電子郵件」
* 沒有工作流程或觸發器對「類型」欄位的值採取動作

## 設定 {#setup}

首先檢查您是否有正確的選擇清單值。 您需要Salesforce管理員的協助，才能對您的選擇清單進行任何變更。

1. 導覽至 [Salesforce.com](https://salesforce.com) 然後按一下右上角的「設定」 。
1. 按一下自訂。
1. 按一下「活動」。
1. 按一下「任務欄位」。
1. 按一下「類型」。
1. 您現在位於任務類型選擇清單中。 請確定未選取「預設」。
1. 請確定「電子郵件」、「呼叫」和「回覆」的「類型」值已列出。

現在，您將開始看到「類型」欄位填入記錄電子郵件、呼叫和回覆的對應值。 這些值將 **not** 在Sales Connect提醒任務中填充。

>[!NOTE]
>
>如果您沒有看到「回覆」值，請按一下 **新增**. 「回覆」不是Salesforce中的標準值。
