---
unique-page-id: 2359500
description: 瞭解分段順序優先順序，以及它如何判斷個人屬於哪個區段。 編輯資料庫中的區段順序以控制區段的評估。
title: 細分順序優先順序
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
TQID: https://experienceleague.adobe.com/wDvufJzxu0BFCSov4etUpEMxaol3-R5CePqllYyDeSc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 140
ht-degree: 4%

---

# 細分順序優先順序 {#segmentation-order-priority}

瞭解&#x200B;**訂單**&#x200B;如何設定分段中人員評估的優先順序很重要。

>[!PREREQUISITES]
>
>[建立細分](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
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
