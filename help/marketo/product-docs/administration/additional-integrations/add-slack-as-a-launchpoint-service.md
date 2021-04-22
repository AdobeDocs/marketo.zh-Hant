---
unique-page-id: 12983619
description: 將Slack新增為LaunchPoint服務-Marketo文檔——產品文檔
title: 將Slack新增為LaunchPoint服務
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 將Slack添加為LaunchPoint服務{#add-slack-as-a-launchpoint-service}

Slack整合包含兩種通知類型：

* **系統通知**:取得有關Marketo例項中重要事件的Slack通知，例如有關目前促銷活動狀態的警報以及任何需要立即注意的問題（CRM錯誤和API限制）。
* **有趣的時刻**:當銷售帳戶中的已知個人觸發Marketo洞察力時，潛在客戶擁有者可透過Slack收到通知。通知包括銷售線索資訊和銷售帳戶的詳細資訊。

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>如果您尚未啟用Slack系統通知，請與[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)聯繫。

1. 前往&#x200B;**LaunchPoint**，然後在&#x200B;**New**&#x200B;下，按一下「New Service」（新服務）**。**

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. 輸入Slack整合的顯示名稱。 在&#x200B;**服務**&#x200B;下拉式清單中，選擇&#x200B;**Slack**。 按一下&#x200B;**建立**。

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. 按一下&#x200B;**授權**。 這會在新標籤中開啟Slack，您將在此處完成授權並授予Marketo從Slack提取資訊的權限。

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. 在新的Slack頁籤中，輸入工作區的URL，然後按一下&#x200B;**繼續**。

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. 輸入您的Slack憑證，然後按一下&#x200B;**登入**。

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. 在&#x200B;**貼文至**&#x200B;下拉式清單中，選取您要張貼來自Marketo的通知的頻道。 檢閱要求的權限，然後按一下「授權&#x200B;**」。**

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. 您應該會看到下方的確認畫面。 頁籤自動關閉。

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. 重新整理「Marketo」標籤，並確認Slack現在已列為LaunchPoint中的作用中服務。

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   通知現在會開始張貼至您在步驟6中選取的渠道。 它們看起來會像這樣：

   ![](assets/samplenotification.png)
