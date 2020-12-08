---
unique-page-id: 2359449
description: 定義區段規則——行銷檔案——產品檔案
title: 定義區段規則
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# 定義區段規則 {#define-segment-rules}

定義區段規則可讓您將人員分為不同的互斥群組。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**必要條件**
>
>[建立區段](create-a-segmentation.md)

1. 轉至數 **據庫。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. 按一下樹狀結構中的**區段**，然後按一下特定 **區段**。

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 按一下「智 **能清單** 」並添加篩選器。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >區段目前不支援 *過去和* *時間範圍*運算子的篩選。 這是因為區段只會在記錄變更資料值時檢查更新。 這些值不 *會記錄* 自動變更的項目，例如公式欄位和日期。 此外，不支援具有相對日期範圍的日期運算子，因為這些運算子是在分段核準時計算，而非在「變更資料值」活動時計算。

   >[!NOTE]
   >
   >「SFDC類型」和「Microsoft類型」篩選器目前在分段智慧清單中不受支援。

1. 為篩選器填寫適當的值。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >**深入探討**
   >
   >
   >智慧型清單非常棒。 瞭解智慧型清單和靜 [態清單的功能](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)。

1. 按一下「 **人員（草稿）** 」標籤，檢視可能符合此區段成員資格的人員。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. 前往區 **段動作**。 按一 **下核准**。

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >您可以在區段中建立的區段總數，取決於所使用的篩選器數目和類型，以及區段邏輯的複雜程度。 雖然您可以使用標準欄位建立最多100個區段，但使用其他類型的篩選器會增加複雜性，而且您的區段可能無法核准。 例如：自訂欄位、清單成員、潛在客戶擁有者欄位和收入階段。
   >
   >
   >如果您在核准期間收到錯誤訊息，並需要協助降低區段的複雜性，請連絡 [Marketo支援](http://nation.marketo.com/t5/Support/ct-p/Support)。

1. 請查看控制面板，以快速概述圓形圖中的區段，以及套用的規則。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

幹得好！ 在Marketo的許多地方，這些區段都會派上用場。

>[!NOTE]
>
>個人可能符合不同區段的資格，但最終只屬於依區段優先順 [序而定的區段](segmentation-order-priority.md)。

>[!NOTE]
>
>**提醒**
>
>「人員（草稿）」畫面會顯示所有符合會員資格且並非總是最終人員清單的人員。 核准您的區段以查看最終清單。

>[!NOTE]
>
>**相關文章**
>
>* [核准區段](approve-a-segmentation.md)

>



