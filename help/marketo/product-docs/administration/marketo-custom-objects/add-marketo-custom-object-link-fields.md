---
unique-page-id: 10097613
description: 新增Marketo自訂物件連結欄位 — Marketo檔案 — 產品檔案
title: 新增Marketo自訂物件連結欄位
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 1dbe820e126f92ce5820e38414925605372a4b09
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# 新增Marketo自訂物件連結欄位 {#add-marketo-custom-object-link-fields}

當您建立自訂物件時，您必須提供連結欄位，以將自訂物件記錄連線到正確的父記錄。

* 對於一對多自訂結構，使用自訂物件中的連結欄位來將其連線到個人或公司。
* 對於多對多的結構，您可以使用兩個連結欄位，由單獨建立的中介物件（也是自訂物件型別）連線。 一個連結會連線至資料庫中的人員或公司，另一個連結則連線至自訂物件。 在這種情況下，連結欄位不在自訂物件本身中。

>[!IMPORTANT]
>
>在多對多關係中，Marketo Engage只支援每個bridge物件的單一edge物件。 在下方提供的範例中，每個註冊只能連結至單一課程。 不過，每個Edge物件可以有許多橋接物件，正如每個課程都有許多學生註冊（多對一關係）。 如果您的自訂物件資料結構化，讓每個Edge物件記錄（一對多或多對多）都有一筆以上的Bridge物件記錄，您可以建立多個Bridge物件記錄，讓每筆記錄都參照單一Edge物件記錄，以便在Marketo中代表該資料。

## 建立一對多結構的連結欄位 {#create-a-link-field-for-a-one-to-many-structure}

以下說明如何在自訂物件中建立一對多結構的連結欄位。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. 按一下&#x200B;**[!UICONTROL Marketo自訂物件]**。

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. 在清單中選取自訂物件。

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. 在&#x200B;**[!UICONTROL 欄位]**&#x200B;索引標籤中，按一下&#x200B;**[!UICONTROL 新增欄位]**。

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. 為連結欄位命名並新增選用的[!UICONTROL 描述]。 請務必選取[!UICONTROL 連結]資料型別。

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >自訂物件獲得核准後，您將無法返回建立、編輯或刪除[!UICONTROL 連結]或[!UICONTROL 重複資料刪除欄位]。

1. 選取[!UICONTROL 連結物件]是針對[!UICONTROL 銷售機會] （人員）還是[!UICONTROL 公司]。

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >如果您選擇[!UICONTROL 銷售機會]，您會在清單中看到ID、電子郵件地址及任何自訂欄位。
   >
   >如果選擇[!UICONTROL 公司]，您會在清單中看到ID與任何自訂欄位。

1. 選取您要連線的[!UICONTROL 連結欄位]作為新欄位的父系。

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >連結欄位僅支援字串欄位型別。

1. 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## 為多對多結構建立連結欄位 {#create-a-link-field-for-a-many-to-many-structure}

以下說明如何在中介物件中建立連結欄位，以用於多對多結構。

>[!PREREQUISITES]
>
>您必須已建立中介物件以及您想要連結至該中介物件的任何自訂物件。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. 按一下&#x200B;**[!UICONTROL Marketo自訂物件]**。

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. 選取您要新增欄位的中介物件。

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. 在&#x200B;**[!UICONTROL 欄位]**&#x200B;索引標籤中，按一下&#x200B;**[!UICONTROL 新增欄位]**。

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. 您必須建立兩個連結欄位。 逐一建立一個。 首先，為資料庫清單成員的欄位命名（例如leadID）。 新增選用的[!UICONTROL 描述]。 請務必選取[!UICONTROL 連結] [!UICONTROL 資料型別]。

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >自訂物件獲得核准後，您將無法返回建立、編輯或刪除[!UICONTROL 連結]或[!UICONTROL 重複資料刪除欄位]。

1. 從您的資料庫選取[!UICONTROL 連結物件]；在此案例中是[!UICONTROL 銷售機會]。

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. 選取您要連線的[!UICONTROL 連結欄位]，在此案例中為[!UICONTROL Id]。

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >[!UICONTROL 連結欄位]僅支援字串欄位型別。

1. 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. 對自訂物件的第二個連結（在此範例中為courseID）重複此程式。 [!UICONTROL 連結物件]名稱將會是course，而[!UICONTROL 連結欄位]將會是courseID。 由於您已建立並核准課程自訂物件，因此可在下拉式功能表中使用這些選項。

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
