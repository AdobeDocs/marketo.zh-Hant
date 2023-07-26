---
unique-page-id: 14352476
description: 任務(SFDC)上的活動型別欄位 — Marketo檔案 — 產品檔案
title: 作業型別欄位(SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 作業型別欄位(SFDC) {#activity-type-field-on-tasks-sfdc}

藉助Sales Connect，您可以在Salesforce中將您的電子郵件和通話記錄為活動。 在Salesforce中有寶貴資料的關鍵部分在於，讓「型別」欄位填入正確的值。

>[!NOTE]
>
>透過「密件副本」記錄電子郵件不會檢視「工作型別」選擇清單，而是會自動將型別欄位填入為「電子郵件」，因為這些電子郵件會透過您的「密件副本」地址傳送給Salesforce。

## 需求 {#requirements}

* 與Salesforce的連線
* 任務型別選擇清單上未選取預設型別值
* 「通話」、「回覆」和「電子郵件」都必須存在於「工作型別」選擇清單下（大寫問題）
* 沒有工作流程或觸發程式對型別欄位的值執行動作

## 設定 {#setup}

首先檢查您是否已準備好正確的挑選清單值。 您需要Salesforce管理員的協助，才能對挑選清單進行任何變更。

1. 瀏覽至 [Salesforce.com](https://salesforce.com) 然後按一下右上角的「設定」 。
1. 按一下「自訂」。
1. 按一下「活動」 。
1. 按一下「工作列位」。
1. 按一下「型別」。
1. 您現在位於工作型別選擇清單。 確認未選取「預設」。
1. 請確定已針對「電子郵件」、「通話」和「回覆」列出「型別」值。

完成設定後，您就會開始看到「型別」欄位填入記錄的電子郵件、來電和回覆的對應值。 這些值會 _非_ 填入Sales Connect提醒工作中。

>[!NOTE]
>
>如果您沒有看到「回覆」值，請按一下以將其新增 **新增**. &#39;Reply&#39;不是Salesforce中的標準值。
