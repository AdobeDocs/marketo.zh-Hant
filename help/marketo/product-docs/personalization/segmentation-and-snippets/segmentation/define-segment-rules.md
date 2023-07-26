---
unique-page-id: 2359449
description: 定義區段規則 — Marketo檔案 — 產品檔案
title: 定義區段規則
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 定義區段規則 {#define-segment-rules}

定義區段規則可讓您將人員分類為不同的互斥群組。

>[!PREREQUISITES]
>
>[建立細分](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. 前往 **資料庫。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. 選取 **細分** 在樹狀結構中，然後按一下特定的 **區段**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 按一下 **智慧清單** 並新增篩選器。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >目前不支援的區段 _過去_ 和 _在時間範圍內_  篩選器上的運運算元。 這是因為區段只會在記錄變更資料值時檢查更新。 這些值為 _非_ 已記錄會自動變更的專案，例如公式欄位和日期。 此外，不支援具有相對日期範圍的日期運運算元，因為這些運運算元是在細分核準時計算，而不是在「變更資料值」活動時計算。

   >[!NOTE]
   >
   >分段智慧清單目前不支援「SFDC型別」和「Microsoft型別」篩選器。

1. 為篩選器填入適當的值。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >帳戶欄位的活動記錄行為可能會影響資格。 因此，我們建議不要在定義區段規則時使用「科目」欄位。

1. 按一下 **人員（草稿）** 標籤來檢視可能符合此區段成員資格的人員。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. 前往 **分段動作**. 按一下 **核准**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >您可以在區段中建立的區段總數，會根據使用的篩選器數量和型別，以及區段的邏輯複雜程度而定。 雖然您可以使用標準欄位建立最多100個區段，但使用其他型別的篩選器可能會增加複雜性，且您的區段可能無法核准。 範例包括：自訂欄位、清單成員、潛在客戶擁有者欄位和收入階段。
   >
   >如果您在核准期間收到錯誤訊息，且需要協助以降低細分複雜度，請聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 請檢視儀表板，以快速瞭解圓餅圖中的區段概況以及套用的規則。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

做得好！ 這些區段在Marketo的許多地方都會派上用場。

>[!NOTE]
>
>個人可能符合不同區段的資格，但最終僅屬於一個區段，這取決於 [區段的優先順序](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>「人物（草稿）」畫面會顯示所有符合成員資格的人，而且不一定是最終的人物清單。 核准您的區段以檢視最終清單。

>[!MORELIKETHIS]
>
>[核准分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
