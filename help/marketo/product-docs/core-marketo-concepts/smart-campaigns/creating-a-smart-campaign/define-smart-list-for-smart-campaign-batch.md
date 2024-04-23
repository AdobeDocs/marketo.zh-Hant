---
unique-page-id: 1146940
description: 定義Smart Campaign的智慧清單 | 批次 — Marketo檔案 — 產品檔案
title: 定義Smart Campaign的智慧清單 | 批次
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# 定義Smart Campaign的智慧清單 | 批次 {#define-smart-list-for-smart-campaign-batch}

智慧列示是整個Marketo Engage用來定義「誰」（哪些人員）的機制，無論是報表、清單或智慧行銷活動皆然。 以下說明如何定義批次行銷活動的智慧清單。

>[!CAUTION]
>
>對作用中行銷活動進行智慧清單或流量步驟編輯可能會破壞其功能。 如果您選擇這麼做，請謹慎操作。

1. 選擇智慧型行銷活動，然後按一下 **[!UICONTROL 智慧清單]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 輸入以搜尋篩選器，並將其拖放至畫布。 對多個篩選器重複此動作。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >僅包含篩選器的智慧型行銷活動執行於 _批次_ 模式。 它會根據篩選器在資料庫中找出符合資格的人員，並一次透過流程執行所有人員。

   >[!NOTE]
   >
   >您可以新增觸發程式，讓Smart Campaign根據即時事件逐人執行 _觸發_ 模式。

1. 按一下下拉式清單，並為您選擇的篩選器選擇篩選器運運算元。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >紅色曲線表示錯誤或遺失資訊。 如果未更正，此行銷活動將會無效且無法執行。

1. 輸入篩選值。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >依預設，符合所有「智慧列示」規則的人皆為合格者。 您可修改以符合行銷活動需求。 簽出  [複雜邏輯的智慧清單規則](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} 以進一步瞭解。

   若要一次觸發一個人的即時活動，請瞭解如何 [定義Smart Campaign的智慧清單 | 觸發](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [定義Smart Campaign的智慧清單 | 觸發](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [將流量步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
