---
unique-page-id: 37356429
description: 在Microsoft —— 行銷檔案——產品檔案中建立工作
title: 在Microsoft中建立任務
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# 在Microsoft中建立任務 {#create-task-in-microsoft}

身為行銷人員，您有可協助銷售人員完成交易的資訊。 您可以建立工作，讓他們知道應該做什麼，以及何時應該做。

在Microsoft中建立任務在Microsoft中與人員（銷售線索或聯繫人）相關的活動下建立一個任務。

>[!NOTE]
>
>此流量步驟僅在 **智慧型促銷活動中與觸發器搭配使用**，而非篩選器搭配使用時有效。

依預設，流程步驟會如下所示：   ![](assets/msd1.png)

>[!NOTE]
>
>當Marketo Sync使用者建立工作時，**Due In **是在Microsoft中建立工作的必填欄位。 如果未輸入值，Marketo預設會輸入5天。

自訂所有欄位，以您想要的方式建立工作。   ![](assets/msd2.png)

>[!NOTE]
>
>為「流動操作」中的任務指定的欄位「狀態」將更新該欄位：Microsoft中的「狀態原因」。

>[!TIP]
>
>您可以在「主 `{{lead.tokens}}`題」和「說明」中使 `{{company.tokens}}`用「主題 `{{campaign.tokens}}` 」和「說 `{{system.tokens}}`********&#x200B;明」。 如需詳 [細資訊，請參閱](http://docs.marketo.com/x/c4AR) 「流程步驟的Token」。

