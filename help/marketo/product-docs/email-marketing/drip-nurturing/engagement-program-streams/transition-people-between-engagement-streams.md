---
unique-page-id: 2359947
description: 在參與資料流之間轉換人員 — Marketo檔案 — 產品檔案
title: 在參與資料流之間轉變人物
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 在參與資料流之間轉變人物 {#transition-people-between-engagement-streams}

參與計畫可以有一個以上的資料流。 如果您[新增資料流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)，您將想要定義讓人員從一個資料流移至另一個資料流的方法。 這些稱為&#x200B;**轉換規則。**

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/ma.png)

1. 選取您的多重串流參與方案，並移至&#x200B;**[!UICONTROL Streams]**。

   ![](assets/multistream.jpg)

1. 按一下您要從其他資料流提取之資料流的&#x200B;**[!UICONTROL Transition Rules]**，然後按一下&#x200B;**[!UICONTROL Edit Transition Rules]**。

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >轉換規則提取到資料流中；請一律在您要提取的資料流上定義規則。

   轉換規則視窗開啟後，在您選擇的觸發程式中尋找並拖曳。 在此案例中，我們想在新增至商機時將人員移至[!UICONTROL Mid Stage]。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 讓我們將運運算元設為&#x200B;**[!UICONTROL is any]**，讓人員移動以取得任何新增的機會。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >您可以將多個觸發器和篩選器新增至轉變規則，但轉變規則會使用所有篩選器（唯一選項是使用「全部」篩選器）。 如果您需要在轉變規則中使用OR，建議您改為設定外部智慧行銷活動。

1. 按一下「**[!UICONTROL Close]**」。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   太棒了！ 現在，參與方案中新增至商機的任何人都將移至[!UICONTROL Mid Stage]資料流。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上述步驟&#x200B;*do*&#x200B;也適用於暫停時[的人員](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)。
