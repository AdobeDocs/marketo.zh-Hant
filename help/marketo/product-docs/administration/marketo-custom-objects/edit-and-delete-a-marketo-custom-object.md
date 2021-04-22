---
unique-page-id: 10093690
description: 編輯和刪除Marketo自訂物件-Marketo檔案——產品檔案
title: 編輯和刪除Marketo自定義對象
exl-id: 97bae63e-f679-490b-bfa2-51d88355b29c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 編輯和刪除Marketo自定義對象{#edit-and-delete-a-marketo-custom-object}

>[!NOTE]
>
>一旦批准自定義對象，就不能建立、編輯或刪除連結或重複資料刪除欄位。

## 編輯自訂物件{#edit-a-custom-object}

使用「自訂物件動作」功能表可編輯或刪除自訂物件。

1. 按一下&#x200B;**Admin**，在&#x200B;**資料庫管理**&#x200B;中，選擇&#x200B;**Marketo自定義對象**。

   ![](assets/image2016-1-18-13-3a31-3a51.png)

1. 選擇您要在右側編輯的自訂物件。

   ![](assets/image2016-1-18-13-3a33-3a11.png)

1. 按一下&#x200B;**自定義對象操作**&#x200B;頁籤，然後按一下&#x200B;**編輯對象**。

   ![](assets/image2015-9-23-11-3a37-3a44.png)

   >[!NOTE]
   >
   >「編輯物件」顯示的欄位與「建立物件」相同，但API名稱是無法編輯的。

1. 進行任何變更。 如果要在「銷售線索詳細資訊」頁上顯示對象，請將滑塊拖動到上方。 按一下&#x200B;**保存**。

   ![](assets/image2015-9-15-16-3a48-3a39.png)

1. 請務必批准[已編輯的對象](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)。

## 刪除自定義對象{#delete-a-custom-object}

刪除自訂物件很簡單，但您必須小心。 自訂物件可連接至其他物件或智慧型清單。 因此，Marketo會先警告您，然後再讓您按一下&#x200B;**Delete**。

>[!CAUTION]
>
>刪除自訂物件後，便無法復原。

1. 按一下&#x200B;**Admin**，在&#x200B;**資料庫管理**&#x200B;中，選擇&#x200B;**Marketo自定義對象**。

   ![](assets/image2016-1-18-13-3a36-3a0.png)

1. 選擇要刪除的對象。

   ![](assets/image2015-9-23-16-3a29-3a5.png)

1. 按一下&#x200B;**自定義對象操作**&#x200B;並選擇&#x200B;**刪除對象**。

   ![](assets/image2015-9-23-11-3a39-3a5.png)

   >[!TIP]
   >
   >您也可以按一下右鍵該對象，然後選擇&#x200B;**刪除對象**。

1. 如果自訂物件為草稿形式，但尚未核准，您會收到此警告。 如果您確定，請按一下「刪除」。****

   ![](assets/image2015-9-23-16-3a31-3a2.png)

1. 如果自訂物件已獲核准，則刪除它時風險較大。 你會得到這個嚴重警告的。 輸入&#x200B;**I deltent**，選中&#x200B;**Cannot Undo**&#x200B;複選框，然後按一下&#x200B;**Delete**。

   ![](assets/image2016-1-15-9-3a49-3a38.png)

   >[!NOTE]
   >
   >如果自定義對象連結到中間對象，則必須先刪除中間對象。

>[!MORELIKETHIS]
>
>[批准自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
