---
unique-page-id: 1146940
description: 定義Smart Campaign的智慧清單 |批次 — Marketo檔案 — 產品檔案
title: 定義Smart Campaign的智慧清單 |批次
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 定義Smart Campaign的智慧清單 |批次 {#define-smart-list-for-smart-campaign-batch}

智慧列示是整個Marketo定義「誰」（哪些人員）的機制，無論是報表、清單或智慧行銷活動皆然。 以下說明如何定義批次行銷活動的智慧清單。

1. 選擇智慧型行銷活動，然後按一下 **智慧清單**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 輸入以搜尋篩選器，並將其拖放到畫布上。 對多個篩選器重複此動作。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >只有篩選器的智慧行銷活動執行於 **批次** 模式。 它會根據篩選器在資料庫中尋找符合條件的人員，並一次透過流程執行所有篩選器。

   >[!NOTE]
   >
   >您可以新增觸發程式，讓Smart Campaign根據即時事件逐人執行 **觸發** 模式。

1. 按一下下拉式清單，並為您選擇的篩選器選擇篩選器運運算元。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >紅色曲折線表示錯誤或遺失資訊。 如果未更正，行銷活動將無效且將無法執行。

1. 輸入篩選值。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >依預設，符合所有「智慧列示」規則的人都是合格的。 您可修改此專案，以符合您的行銷活動需求。 簽出  [複雜邏輯的智慧清單規則](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) 以深入瞭解。

   若要逐一觸發即時活動，請瞭解如何 [定義Smart Campaign的智慧清單 |觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [定義Smart Campaign的智慧清單 |觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [將流量步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
