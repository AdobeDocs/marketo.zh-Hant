---
unique-page-id: 10093192
description: 建立Marketo自訂物件 — Marketo檔案 — 產品檔案
title: 建立Marketo自訂物件
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# 建立Marketo自訂物件 {#create-marketo-custom-objects}

使用Marketo中的自訂物件來追蹤您業務的特定量度。 從汽車到課程，這可能是任何事情 — 無論您想在Marketo中建立何種模型來執行行銷活動。

>[!NOTE]
>
>您可以設定自訂物件以一對多或多對多運作。 您可以使用相同的方式建立初始對象，但開始向對象添加欄位時，步驟不同。 請參閱  [了解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以取得更多資訊。

>[!NOTE]
>
>批准自定義對象後，您就無法建立、編輯或刪除連結或重複資料刪除欄位。

## 為一對多結構建立自訂物件 {#create-a-custom-object-for-a-one-to-many-structure}

此範例顯示用於一對多結構的Car自訂物件。 之後，您將建立一個課程自定義對象和一個中間對象，以用於多對多結構。

1. 前往 **管理** 的上界。

   ![](assets/create-marketo-custom-objects-1.png)

1. 按一下 **Marketo自訂物件**.

   ![](assets/create-marketo-custom-objects-2.png)

1. 按一下 **新自訂物件**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >「Marketo自訂物件」索引標籤會在右側顯示所有自訂物件，以及任何已核准物件的詳細資訊，包括最新更新時的記錄數和欄位數。

1. 輸入顯示名稱。 API名稱和複數名稱會自動填入。 輸入說明（可選）。

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >建立這些欄位時，您可以編輯這些欄位，但儲存後，您只能編輯「複數名稱」欄位和 **顯示在銷售線索詳細資訊中** 滑桿。

1. 提取 **顯示在銷售線索詳細資訊中** 滑過以顯示 **顯示** 如果要在「資料庫」頁上查看自定義對象資料。 按一下 **儲存**.

   ![](assets/create-marketo-custom-objects-5.png)

1. 自訂物件資訊會顯示您輸入的內容。 注意它處於草稿狀態。

   ![](assets/create-marketo-custom-objects-6.png)

   下一步是將欄位新增至 [建置自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >您只能透過清單匯入填入Marketo自訂物件，或 [API](https://developers.marketo.com/documentation/rest/).

## 為多對多結構建立自訂物件 {#create-a-custom-object-for-a-many-to-many-structure}

此示例顯示一個課程自定義對象，您將用它在人員/公司和課程之間建立多對多關係。 完成後，您將建立一個中間對象以將其連接到資料庫中的人員或公司。

>[!NOTE]
>
>對於多對多關係，您不需要在自訂物件中建立連結。 相反地，您會新增兩個連結至中繼物件（請參閱下方）。

1. 前往 **管理** 的上界。

   ![](assets/create-marketo-custom-objects-7.png)

1. 按一下 **Marketo自訂物件**.

   ![](assets/create-marketo-custom-objects-8.png)

1. 按一下 **新自訂物件**.

   ![](assets/create-marketo-custom-objects-9.png)

1. 輸入顯示名稱。 API名稱和複數名稱會自動填入。 輸入說明（可選）。

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >建立這些欄位時，您可以編輯這些欄位，但儲存後，您只能編輯「複數名稱」欄位和 **顯示在銷售線索詳細資訊中** 滑桿。

1. 提取 **顯示在銷售線索詳細資訊中** 滑過以顯示 **顯示** 如果要在「資料庫」頁上查看自定義對象資料。 按一下 **儲存**.

   ![](assets/create-marketo-custom-objects-11.png)

1. 自訂物件資訊會顯示您輸入的內容。 注意它處於草稿狀態。

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >您只能透過清單匯入填入Marketo自訂物件，或 [API](https://developers.marketo.com/documentation/rest/).

下一步是建立中繼物件（請參閱下方）。 但在此之前，您需要建立一個欄位以連結至。

## 建立中繼物件 {#create-an-intermediary-object}

使用中繼物件將自訂物件連結至人員或公司。 在此示例中，它用於將課程中的課程自定義對象與資料庫中的人員或公司連接起來。

>[!NOTE]
>
>您不需要為一對多自訂物件結構建立中介物件。

1. 前往 **管理** 的上界。

   ![](assets/create-marketo-custom-objects-13.png)

1. 按一下 **Marketo自訂物件**.

   ![](assets/create-marketo-custom-objects-14.png)

1. 按一下 **新自訂物件**.

   ![](assets/create-marketo-custom-objects-15.png)

1. 輸入顯示名稱。 API名稱和複數名稱會自動填入。 輸入說明（可選）。

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >在建立這些欄位時，您可以編輯這些欄位，但在儲存後，您只能編輯「複數名稱」欄位和「顯示在銷售機會詳細資訊」滑桿。

1. 提取 **顯示在銷售線索詳細資訊中** 滑過以顯示 **顯示** 如果要在「資料庫」頁上查看自定義對象資料。 按一下 **儲存**.

   ![](assets/create-marketo-custom-objects-17.png)

1. 自訂物件資訊會顯示您輸入的內容。 注意它處於草稿狀態。

   下一步是讓您 [新增連結欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) 將中介物件連結至人員/公司和自訂物件。

>[!MORELIKETHIS]
>
>* [新增Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [新增Marketo自訂物件連結欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [了解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

