---
unique-page-id: 14352476
description: 任務上的活動型別欄位(SFDC) - Marketo檔案 — 產品檔案
title: 工作的活動類型欄位 (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 7%

---

# 工作的活動類型欄位 (SFDC) {#activity-type-field-on-tasks-sfdc}

在[!DNL Sales Connect]的協助下，您可以在[!DNL Salesforce]中將您的電子郵件和通話記錄為活動。 在[!DNL Salesforce]中有寶貴資料的關鍵部分就是讓[!UICONTROL Type]欄位填入正確的值。

>[!NOTE]
>
>透過密件副本記錄電子郵件將不會尋找「工作型別」選擇清單，而是會自動將型別欄位填入為「電子郵件」，因為這些電子郵件會透過您的密件副本位址傳送至[!DNL Salesforce]。

## 需求 {#requirements}

* 與[!DNL Salesforce]的連線
* 任務型別選擇清單上未選取預設型別值
* 「通話」、「回覆」和「電子郵件」都必須存在於「工作型別」選擇清單下（大寫問題）
* 沒有工作流程或觸發程式對型別欄位的值執行動作

## 設定 {#setup}

首先檢查您是否已準備好正確的挑選清單值。 您需要[!DNL Salesforce]管理員的協助才能變更挑選清單。

1. 導覽至[Salesforce.com](https://salesforce.com)，然後按一下右上角的[設定]。
1. 按一下「**[!UICONTROL Customize]**」。
1. 按一下「**[!UICONTROL Activities]**」。
1. 按一下「**[!UICONTROL Task Fields]**」。
1. 按一下「**[!UICONTROL Type]**」。
1. 您現在位於工作型別選擇清單。 確認未選取「預設」。
1. 確定已列出[!UICONTROL Type]、[!UICONTROL Email]和[!UICONTROL Call]的[!UICONTROL Reply]值。

完成設定後，您就會開始看到「型別」欄位填入記錄的電子郵件、來電和回覆的對應值。 Sales Connect提醒工作將&#x200B;_不會填入這些值_。

>[!NOTE]
>
>如果您沒有看到「回覆」的值，請按一下「**[!UICONTROL New]**」將其新增。 &#39;Reply&#39;不是[!DNL Salesforce]中的標準值。
