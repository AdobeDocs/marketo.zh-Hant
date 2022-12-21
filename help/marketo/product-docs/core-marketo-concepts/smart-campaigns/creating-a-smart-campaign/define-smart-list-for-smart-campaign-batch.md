---
unique-page-id: 1146940
description: 定義智慧促銷活動的智慧清單 |批次 — Marketo檔案 — 產品檔案
title: 定義智慧促銷活動的智慧清單 |批
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 定義智慧促銷活動的智慧清單 |批 {#define-smart-list-for-smart-campaign-batch}

智慧型清單是整個Marketo中定義「誰」（哪些人）要納入的機制，無論是報表、清單或智慧型行銷活動。 以下說明如何為批次促銷活動定義智慧清單。

1. 選擇智慧型促銷活動，然後按一下 **智慧清單**.

   ![](assets/campaignchoose-hand.png)

1. 輸入以搜尋篩選器，然後將其拖放至畫布。 對多個篩選器重複。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >只有篩選器的智慧型行銷活動會在中執行 **批次** 模式。 它會在資料庫中根據篩選條件找到符合資格的人員，並一次透過流程執行所有人員。

   >[!NOTE]
   >
   >您可以透過新增觸發器，根據即時事件，一次在一個人上執行智慧型促銷活動，如此可以放置智慧型促銷活動 **觸發** 模式。

1. 按一下下拉式清單，然後為您選取的篩選選擇篩選運算子。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >紅曲線表示錯誤或缺少資訊。 若未更正，則促銷活動將無效，且不會執行。

1. 輸入篩選值。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >預設情況下，滿足「全部」智慧清單規則的人員是合格的。 您可以修改以符合您的促銷活動需求。 結帳  [複雜邏輯的智慧清單規則](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) 了解更多。

   若要一次觸發一個人的即時事件，請了解如何 [定義智慧促銷活動的智慧清單 |觸發](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [定義智慧促銷活動的智慧清單 |觸發](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [新增流量步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

