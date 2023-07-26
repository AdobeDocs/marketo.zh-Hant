---
unique-page-id: 10097613
description: 新增Marketo自訂物件連結欄位 — Marketo檔案 — 產品檔案
title: 新增Marketo自訂物件連結欄位
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 新增Marketo自訂物件連結欄位 {#add-marketo-custom-object-link-fields}

當您建立自訂物件時，您必須提供連結欄位，以將自訂物件記錄連線到正確的父記錄。

* 對於一對多自訂結構，使用自訂物件中的連結欄位來將其連線到個人或公司。
* 對於多對多的結構，您可以使用兩個連結欄位，由單獨建立的中介物件（也是自訂物件型別）連線。 一個連結會連線至資料庫中的人員或公司，另一個連結則連線至自訂物件。 在這種情況下，連結欄位不在自訂物件本身中。

## 建立一對多結構的連結欄位 {#create-a-link-field-for-a-one-to-many-structure}

以下說明如何在自訂物件中建立一對多結構的連結欄位。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. 按一下 **[!UICONTROL Marketo自訂物件]**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. 在清單中選取自訂物件。

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. 在 **[!UICONTROL 欄位]** 標籤，按一下 **[!UICONTROL 新欄位]**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. 為連結欄位命名並新增選用專案 [!UICONTROL 說明]. 請務必選取 [!UICONTROL 連結] 資料型別。

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >您將無法返回並建立、編輯或刪除 [!UICONTROL 連結] 或 [!UICONTROL 重複資料刪除欄位] 在核准自訂物件之後。

1. 選取是否 [!UICONTROL 連結物件] 針對 [!UICONTROL 銷售機會] （人員）或 [!UICONTROL 公司].

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >如果您選擇 [!UICONTROL 銷售機會]，您會在清單中看到ID、電子郵件地址及任何自訂欄位。
   >
   >如果您選擇 [!UICONTROL 公司]，您會在清單中看到ID及任何自訂欄位。

1. 選取 [!UICONTROL 連結欄位] 您想要以新欄位的父項身份連線到。

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >連結欄位僅支援字串欄位型別。

1. 按一下 **[!UICONTROL 儲存]**.

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## 為多對多結構建立連結欄位 {#create-a-link-field-for-a-many-to-many-structure}

以下說明如何在中介物件中建立連結欄位，以用於多對多結構。

>[!PREREQUISITES]
>
>您必須已建立中介物件以及您想要連結至該中介物件的任何自訂物件。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. 按一下 **[!UICONTROL Marketo自訂物件]**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. 選取您要新增欄位的中介物件。

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. 在 **[!UICONTROL 欄位]** 標籤，按一下 **[!UICONTROL 新欄位]**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. 您必須建立兩個連結欄位。 逐一建立一個。 首先，為資料庫清單成員的欄位命名（例如leadID）。 新增選用專案 [!UICONTROL 說明]. 請務必選取 [!UICONTROL 連結] [!UICONTROL 資料型別].

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >您將無法返回並建立、編輯或刪除 [!UICONTROL 連結] 或 [!UICONTROL 重複資料刪除欄位] 在核准自訂物件之後。

1. 選取 [!UICONTROL 連結物件] 從您的資料庫；在本例中， [!UICONTROL 銷售機會].

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. 選取 [!UICONTROL 連結欄位] 在此情況下，您想要連線至 [!UICONTROL Id].

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >中僅支援字串欄位型別 [!UICONTROL 連結欄位].

1. 按一下 **[!UICONTROL 儲存]**.

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. 對自訂物件的第二個連結（在此範例中為courseID）重複此程式。 此 [!UICONTROL 連結物件] 名稱將會是course，而 [!UICONTROL 連結欄位] 將是courseID。 由於您已建立並核准課程自訂物件，因此可在下拉式功能表中使用這些選項。

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. 建立您要在中介物件中使用的任何其他欄位，例如enrollmentID或等級。

## 使用自訂物件 {#using-custom-objects}

下一步是在您的智慧行銷活動中，於篩選器中使用這些自訂物件。 透過多對多關係，您可以選取多個人員/公司和多個自訂物件。 在下列範例中，資料庫中符合這些條件的任何人都將會列出。 coursename欄位來自課程自訂物件，而註冊等級來自中繼物件。

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [新增Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [編輯和刪除Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [瞭解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [編輯和刪除Marketo自訂物件欄位](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
