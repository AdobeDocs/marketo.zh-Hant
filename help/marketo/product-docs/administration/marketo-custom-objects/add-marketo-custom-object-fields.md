---
unique-page-id: 10093688
description: 新增Marketo自訂物件欄位 — Marketo檔案 — 產品檔案
title: 新增Marketo自訂物件欄位
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 新增Marketo自訂物件欄位 {#add-marketo-custom-object-fields}

建立自訂物件後，您需要新增欄位至該物件，以符合您的業務需求。

欄位會定義自訂物件所使用的特定資訊。 連結欄位有特殊工作，可用來連結自訂物件，且會包含在 [獨立文章](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. 前往 **管理** 的上界。

   ![](assets/add-marketo-custom-object-fields-1.png)

1. 按一下 **Marketo自訂物件**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. 選取您要在右側新增欄位的物件。

   ![](assets/add-marketo-custom-object-fields-3.png)

1. 在 **欄位** 按一下 **新欄位**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Marketo會在您建立自訂物件時自動建立上述三個欄位。 Marketo會自動管理這些欄位，而您無法編輯或刪除這些欄位。

1. 輸入顯示名稱和說明。

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >API名稱只能編輯，直到獲得核准為止。

1. 現在，從清單中選擇適當的資料類型。

   ![](assets/add-marketo-custom-object-fields-6.png)

1. 如果要將新欄位用作唯一標識符，請將重複資料消除滑塊拉過。 按一下 **儲存** 完成。

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >重複資料刪除欄位可用於檢索、更新或刪除自定義對象。 每個自定義對象定義必須至少包含一個（且不超過三個）重複資料消除欄位。

1. 新增您需要的任何其他欄位。

   >[!NOTE]
   >
   >如果您要建立一對多結構，則需要將「連結」欄位新增至自訂物件。 對於多對多結構，自訂物件中不需要連結欄位，但您必須在中間物件中新增兩個連結欄位。 請參閱 [新增Marketo自訂物件連結欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) 建立連結欄位，以及 [了解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) ，以了解有關自定義對象類型的詳細資訊。

>[!MORELIKETHIS]
>
>* [新增Marketo自訂物件連結欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [編輯和刪除Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [編輯和刪除Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [了解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

