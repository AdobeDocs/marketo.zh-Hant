---
unique-page-id: 10093688
description: 新增Marketo自訂物件欄位 — Marketo檔案 — 產品檔案
title: 新增Marketo自訂物件欄位
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 新增Marketo自訂物件欄位 {#add-marketo-custom-object-fields}

建立自訂物件後，您需要新增欄位以符合業務需求。

欄位會定義自訂物件所使用的特定資訊。 連結欄位有特殊工作可連線自訂物件，並且包含在 [個別文章](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/add-marketo-custom-object-fields-1.png)

1. 按一下 **[!UICONTROL Marketo自訂物件]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. 選取您要在右側新增欄位的物件。

   ![](assets/add-marketo-custom-object-fields-3.png)

1. 按一下 **[!UICONTROL 欄位]** 標籤，然後 **[!UICONTROL 新欄位]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >當您建立自訂物件時，Marketo會自動建立以上顯示的三個欄位。 Marketo會自動管理這些欄位，您無法編輯或刪除它們。

1. 輸入 [!UICONTROL 顯示名稱] 和（可選） [!UICONTROL 說明].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >API名稱只能編輯，直到獲得核准為止。

1. 現在，選擇適當的 [!UICONTROL 資料型別] 從清單中。

   ![](assets/add-marketo-custom-object-fields-6.png)

1. 提取 [!UICONTROL 重複資料刪除] 如果要使用新欄位作為唯一識別碼，請將滑桿移到。 按一下 **[!UICONTROL 儲存]** 完成。

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >重複資料刪除欄位可用於擷取、更新或刪除自訂物件。 每個自訂物件定義都必須包含至少一個（但不超過三個）重複資料刪除欄位。

1. 新增您需要的任何其他欄位。

   >[!NOTE]
   >
   >如果您建置一對多結構，則需要將連結欄位新增至自訂物件。 對於多對多結構，自訂物件中不需要連結欄位，但必須在中介物件中新增兩個連結欄位。 另請參閱 [新增Marketo自訂物件連結欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) 以建立連結欄位，以及 [瞭解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以取得自訂物件型別的詳細資訊。

>[!MORELIKETHIS]
>
>* [新增Marketo自訂物件連結欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [編輯和刪除Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [編輯和刪除Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [瞭解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
