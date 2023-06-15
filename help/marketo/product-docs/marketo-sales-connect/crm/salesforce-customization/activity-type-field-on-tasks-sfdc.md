---
unique-page-id: 14352476
description: 任務上的活動型別欄位(SFDC) - Marketo檔案 — 產品檔案
title: 任務上的活動型別欄位(SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 46c48172a58cf6bd2e9772ef57510fd7d808adc2
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 任務上的活動型別欄位(SFDC) {#activity-type-field-on-tasks-sfdc}

在Sales Connect的協助下，您可以將電子郵件和通話記錄為Salesforce中的活動。 在Salesforce中有價值資料的關鍵部分就是讓「型別」欄位填入正確的值。

>[!NOTE]
>
>透過「密件副本」記錄電子郵件不會檢視「任務型別」選擇清單，而是會自動將「型別」欄位填入為「電子郵件」，因為這些電子郵件會透過您的「密件副本」地址傳送到Salesforce。

## 需求 {#requirements}

* 與Salesforce的連線
* 「任務型別」選擇清單中未選取預設型別值
* 「工作型別」選擇清單下必須有「通話」、「回覆」和「電子郵件」（大寫內容）
* 沒有工作流程或觸發器對「型別」欄位的值採取行動

## 設定 {#setup}

首先檢查您是否有正確的挑選清單值。 您需要Salesforce管理員的協助，才能對挑選清單進行任何變更。

1. 導覽至 [Salesforce.com](https://salesforce.com) ，然後按一下右上角的「設定」 。
1. 按一下「自訂」。
1. 按一下「活動」。
1. 按一下「工作列位」。
1. 按一下「型別」。
1. 您現在位於任務型別選擇清單。 確定未選取「預設」。
1. 請確定列出了「電子郵件」、「通話」和「回覆」的「型別」值。

完成設定後，您就會開始看到「型別」欄位填入記錄電子郵件、來電和回覆的對應值。 這些值將 _not_ 填入Sales Connect提醒任務中。

>[!NOTE]
>
>如果您沒有看到「回覆」值，請按一下以新增該值 **新增**. &#39;Reply&#39;不是Salesforce中的標準值。
