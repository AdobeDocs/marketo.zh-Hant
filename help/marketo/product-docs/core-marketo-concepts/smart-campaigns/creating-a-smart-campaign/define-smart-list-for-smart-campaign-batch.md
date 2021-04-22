---
unique-page-id: 1146940
description: 定義智慧型促銷活動的智慧型清單 |批次-Marketo文檔——產品文檔
title: 定義智慧型促銷活動的智慧型清單 |批次
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 定義智慧型促銷活動的智慧型清單 |批{#define-smart-list-for-smart-campaign-batch}

智慧型清單是整個Marketo的機制，可定義要包含的「誰」（哪些人），不論是報表、清單或智慧型促銷活動。 以下是如何定義批次促銷活動的智慧清單。

1. 選擇智慧型促銷活動，然後按一下「智慧型清單」**。**

   ![](assets/campaignchoose-hand.png)

1. 輸入以搜尋篩選，然後拖放至畫布。 對多個濾鏡重複此步驟。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >只有篩選器的智慧型促銷活動會在&#x200B;**Batch**&#x200B;模式中執行。 它會根據篩選條件在資料庫中尋找符合資格的人員，並同時透過流程執行所有篩選條件。

   >[!NOTE]
   >
   >您可以新增觸發器，讓智慧型促銷活動在即時事件的基礎上，一次在一個人上執行，這會將智慧型促銷活動置於&#x200B;**Trigger**&#x200B;模式。

1. 按一下下拉式清單，然後為您選擇的篩選選擇篩選運算子。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >紅色的扭曲線表示錯誤或缺少資訊。 如果未更正，促銷活動將無效且不會執行。

1. 輸入篩選值。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >預設情況下，滿足「全部」智慧清單規則的人員是合格的。 您可以修改此項目以符合您的促銷活動需求。 如需詳細資訊，請參閱[複雜邏輯的智慧清單規則](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)。

   若要一次觸發一個人的即時事件，請瞭解如何[定義智慧型促銷活動的智慧型清單 |觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)。

   >[!MORELIKETHIS]
   >
   >* [定義智慧型促銷活動的智慧型清單 |觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [新增流量步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

