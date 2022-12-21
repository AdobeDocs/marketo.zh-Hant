---
unique-page-id: 1146978
description: 使用等待流程步驟的持續時間 — Marketo檔案 — 產品檔案
title: 在等待流程步驟中使用持續時間
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 在等待流程步驟中使用持續時間 {#use-a-duration-in-a-wait-flow-step}

您可以使用「等待流程」步驟，將人員的歷程暫停一段特定時間的智慧促銷活動。 您也可以指定一週中某天的條件，以及結束的時間。

1. 在您的智慧行銷活動中 **流量** 標籤，拖曳至 **等待** 流程步驟。

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. 輸入要暫停的時間。

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. 就這樣！ 流程會在您指定的持續時間中暫停。 如需進階選項，請按一下右側的齒輪圖示。

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. 指定等候步驟應結束的一週中哪一天。

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. （可選）指定時間。 按一下 **儲存**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**範例**
   >
   >週五下午5點，某人觸發了智慧型行銷活動。 等待步驟為進階：48小時，必須在週一至週五早上9點結束。
   >
   >結果是，該人將繼續 **星期一，上午9點**. 這是48小時後的第一次M-F約會。

   >[!NOTE]
   >
   >使用的持續時間、日期、時間和天數皆根據訂閱的時區而定。

   >[!MORELIKETHIS]
   >
   >* [在等待流程步驟中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [在等待流程步驟中使用日期代號](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)

