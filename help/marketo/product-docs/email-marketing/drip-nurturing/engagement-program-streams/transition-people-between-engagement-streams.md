---
unique-page-id: 2359947
description: 在參與串流之間轉變人物 — Marketo檔案 — 產品檔案
title: 在參與串流之間轉換人員
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 在參與串流之間轉換人員 {#transition-people-between-engagement-streams}

參與計畫可以有一個以上的串流。 若您 [新增資料流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)，您會想要定義人們在不同資料流之間移動的方式。 這些稱為 **轉變規則。**

1. 前往 **行銷活動**.

   ![](assets/ma.png)

1. 選取您的多串流參與計畫，並前往 **串流**.

   ![](assets/multistream.jpg)

1. 按一下 **轉換規則** 針對您要從其他資料流提取到的資料流，然後按一下 **編輯轉變規則**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >轉變規則提取到資料流中；一律定義您要提取到之資料流中的規則。

   轉換規則視窗開啟後，在您選擇的觸發器中尋找並拖曳。 在此案例中，我們希望在新增至機會時，將使用者移至「中段」。

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. 讓我們將運運算元設為 **為任何** 讓人員移動以取得任何新增的機會。

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >您可以將多個觸發器和篩選器新增至轉變規則，但轉變規則會使用所有篩選器（使用「全部」篩選器是唯一選項）。 如果您需要在轉變規則中使用OR，建議您改為設定外部智慧行銷活動。

1. 按一下 **關閉**。

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   太棒了！ 現在，您參與方案中新增至商機的任何人都將移至中段資料流。

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >上述步驟 *do* 適用於以下人員： [暫停時](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) 以及。
