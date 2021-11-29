---
unique-page-id: 2359449
description: 定義區段規則 — Marketo檔案 — 產品檔案
title: 定義區段規則
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 定義區段規則 {#define-segment-rules}

「定義區段規則」可讓您將使用者分類為不同的互斥群組。

>[!PREREQUISITES]
>
>[建立區段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. 前往 **資料庫。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. 選擇 **區段** 從樹中，按一下特定 **區段**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 按一下 **智慧清單** 和新增篩選器。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >區段目前不支援 _過去_ 和 _時間範圍_  運算子。 這是因為區段只會在記錄變更資料值時檢查更新。 這些值包括 _not_ 記錄自動變更的項目，例如公式欄位和日期。 此外，不支援具有相對日期範圍的日期運算子，因為這些運算子是在分段核準時計算，而不是在「變更資料值」活動時計算。

   >[!NOTE]
   >
   >「SFDC類型」和「Microsoft類型」篩選器目前在分段智慧清單中不受支援。

1. 為篩選器填入適當的值。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >「帳戶」欄位的活動記錄行為可能會影響資格。 因此，在定義區段規則時，我們建議不要使用「帳戶」欄位。

1. 按一下 **人員（草稿）** 頁簽來查看可能符合此段成員資格的人員。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. 前往 **區段動作**. 按一下 **核准**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >您可在區段中建立的區段總數，取決於使用的篩選器數目和類型，以及區段邏輯的複雜程度。 雖然您可以使用標準欄位建立最多100個區段，但使用其他類型的篩選器可能會增加複雜度，而您的區段可能無法核准。 例如：自訂欄位、清單成員、銷售機會擁有者欄位和收入階段。
   >
   >如果您在核准期間收到錯誤訊息，並需要協助降低區段的複雜性，請聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 查看控制面板，快速概述圓形圖中的區段，以及套用的規則。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

幹得好！ 這些區段在Marketo的很多地方都會派上用場。

>[!NOTE]
>
>人員可能符合不同區段的資格，但最終只屬於依 [區段的優先順序](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>「人員（草稿）」畫面會顯示所有符合成員資格的人員，且並不總是人員的最終清單。 核准您的區段以查看最終清單。

>[!MORELIKETHIS]
>
>[核准區段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
