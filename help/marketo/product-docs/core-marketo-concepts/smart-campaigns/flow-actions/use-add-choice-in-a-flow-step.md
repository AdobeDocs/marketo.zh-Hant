---
unique-page-id: 1146980
description: 在流程步驟中使用新增選擇 — Marketo檔案 — 產品檔案
title: 在流程步驟中使用新增選項
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# 在流程步驟中使用新增選項 {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[將流程步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

「新增選擇」可讓您使用流程步驟，並在選擇詳細資料時顯示「視情況而定」。

1. 在Smart Campaign的&#x200B;**[!UICONTROL 流量]**&#x200B;標籤下，新增任何流量步驟，然後按一下&#x200B;**[!UICONTROL 新增選擇]**。

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. 選取選擇條件。

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. 選擇選擇運運算元並輸入選擇值。 這會設定您的條件或選擇。

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. 輸入選擇的流程步驟值。

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Token將&#x200B;_無法_&#x200B;在選擇流程步驟的條件部分運作。

1. 重複上述步驟以新增多個選項，然後新增/調整預設值。

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >您可以將任何流程步驟設定為 — 不執行任何動作 — 在此情況下，不會對該選擇採取任何動作。

   >[!CAUTION]
   >
   >只有第一個相符選擇會套用到流程步驟。 瞭解如何在流程動作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}中[重新排序「新增選擇」。

   太棒了！ 您現在可以建立具有流程步驟選擇的單一Smart Campaign，而不是為每個選擇建立多個Smart Campaign。

   >[!MORELIKETHIS]
   >
   >[在流程步驟中重新排序新增選擇](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
