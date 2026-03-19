---
unique-page-id: 2359500
description: 瞭解分段順序優先順序，以及它如何判斷個人屬於哪個區段。 編輯資料庫中的區段順序以控制區段的評估。
title: 細分順序優先順序
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 4%

---

# 細分順序優先順序 {#segmentation-order-priority}

瞭解&#x200B;**訂單**&#x200B;如何設定分段中人員評估的優先順序很重要。

>[!PREREQUISITES]
>
>[建立分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[定義區段規則](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>您只能在草稿模式中編輯分段。

1. 移至&#x200B;**資料庫**。

   ![](assets/segmentation-order-priority-1.png)

1. 選取您的&#x200B;**分段**。 在&#x200B;**[!UICONTROL Segmentation Actions]**&#x200B;中，按一下&#x200B;**[!UICONTROL Edit Segments]**。

   ![](assets/segmentation-order-priority-2.png)

   您可以從此畫面檢查或編輯區段的順序。

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* 這些區段互相排斥。 個人一次只能是一個區段的成員。
>* 當個人符合兩個區段的資格時，他們僅屬於清單中的第一個區段。
>* 如果人員不符合任何區段的資格，他們將成為「預設區段」的成員。
