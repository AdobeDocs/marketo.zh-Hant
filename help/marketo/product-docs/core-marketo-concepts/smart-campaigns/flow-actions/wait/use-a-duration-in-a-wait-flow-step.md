---
unique-page-id: 1146978
description: 在等待流程步驟中使用持續時間 — Marketo檔案 — 產品檔案
title: 在等待流程步驟中使用持續時間
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 1%

---

# 在等待流程步驟中使用持續時間 {#use-a-duration-in-a-wait-flow-step}

您可以使用等待流程步驟，將個人穿過Smart Campaign的歷程暫停一段特定時間。 您也可以指定星期幾的標準以及結束的時間。

1. 在您的Smart Campaign **[!UICONTROL 流量]** 標籤，拖曳至 **[!UICONTROL 等待]** 流程步驟。

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. 輸入您要暫停多久。

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. 完成了！ 流量將在您指定的期間內暫停。 如需進階選項，請按一下右側的齒輪圖示。

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. 指定一週中等待步驟的結束日期。

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. 選擇性地指定時間。 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**範例**
   >
   >有人在星期五下午5點觸發Smart Campaign。 等待步驟已提前：48小時，必須在週一至週五上午9點結束。
   >
   >結果此人將繼續在流量中排名 **星期一上午9點**. 這是48小時後的第一個M-F日期。

   >[!NOTE]
   >
   >使用的持續時間、日期、時間和天數都取決於您的訂閱時區。

   >[!MORELIKETHIS]
   >
   >* [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [在等待流程步驟中使用日期權杖](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
