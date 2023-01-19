---
unique-page-id: 10094188
description: 核准自訂物件 — Marketo檔案 — 產品檔案
title: 核准自訂物件
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 核准自訂物件 {#approve-a-custom-object}

您必須先核准自訂物件，才能加以使用。 新自訂物件和您編輯的物件的程式稍有不同。

## 核准新的自訂物件 {#approve-a-new-custom-object}

您已建立全新的自訂物件。 以下是如何核准。

1. 前往 **管理** 的上界。

   ![](assets/approve-a-custom-object-1.png)

1. 按一下 **Marketo自訂物件**.

   ![](assets/approve-a-custom-object-2.png)

1. 選取處於「草稿」狀態的物件。

   ![](assets/approve-a-custom-object-3.png)

1. 按一下 **自訂物件動作** 下拉式清單並選取 **核准物件**.

   ![](assets/approve-a-custom-object-4.png)

1. 狀態變更為「已核准」。

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >用於 _一對多結構_ 必須至少有一個重複資料刪除欄位、連結欄位、連結對象名稱和要批准的連結欄位名稱。
   >
   >用於 _多對多結構_ **does&#39;t** 在您核准連結欄位、連結的物件名稱或連結的欄位名稱時，都需要連結欄位（因為這些名稱位於中間物件中）。
   >
   >自訂物件，作為 _中介對象_ 需要連結欄位、連結的物件名稱和連結的欄位名稱，但 **does&#39;t** 需要重複資料刪除欄位。
   >
   >請參閱 [了解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以取得更多資訊。

就這樣！ 現在，您可以在篩選器和觸發器的限制中選取自訂物件，以用於行銷活動。

## 核准編輯的自訂物件 {#approve-an-edited-custom-object}

編輯已核准的自訂物件後，您必須核准草稿，將自訂物件傳回「已核准」狀態。

1. 當您編輯已核准的自訂物件時，它會收到「已核准」狀態的草稿。

   ![](assets/approve-a-custom-object-6.png)

1. 準備好核准草稿時，請按一下 **自訂物件動作** 下拉式清單並選取 **核准物件**.

   ![](assets/approve-a-custom-object-7.png)

1. 預覽會顯示在草稿中變更的項目。 按一下 **核准**.

   ![](assets/approve-a-custom-object-8.png)
