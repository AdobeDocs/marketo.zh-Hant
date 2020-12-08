---
unique-page-id: 10099680
description: 匯入自訂物件資料——行銷人員檔案——產品檔案
title: 匯入自訂物件資料
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# 匯入自訂物件資料 {#import-custom-object-data}

將自訂物件資料匯入資料庫十分簡單。 如果您正在公司中使用自訂物件，請參閱在公 [司中使用自訂物件](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies) ，以取得詳細資訊。

1. 在My Marketo中，轉至「數 **據庫**」。

   ![](assets/db-1.png)

1. 按一 **下「新增** 」，然後 **選取「匯入自訂物件資料」**。

   ![](assets/image2016-4-7-10-6-54.png)

1. 按一 **下瀏覽** ，以找出資料檔案。 選取檔案格式（此範例中的逗號分隔值）。

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. 選取您的自訂物件。

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. 從下拉式清單中選擇「重複資料消除模式」。 按一 **下「下一步**」。

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >在建立或更新自定義對象記錄時，使用「重複資料消除」欄位作為唯一標識符。 此示例使用汽車定制對象 **vin** （車輛ID號）的「重複資料刪除」欄位。 如果您只更新自訂物件記錄，可以選取「Marketo Guid」（行銷人員指南）作為重複資料刪除模式。

1. 將每欄對應至Marketo欄位，從下拉式清單中選取欄位。

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >請確定檔案中的值符合您要比對的欄位類型（例如文字、整數等），否則檔案將遭拒。

1. 按一 **下「下一步**」。

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. 按一 **下匯入**。

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >自訂物件的大小限制為100MB。

   >[!TIP]
   >
   >在「傳送警報至」中輸 **入您的電子郵件地址：** 欄位和Marketo會在匯入完成時以電子郵件寄送您！

1. 在螢幕的右上角，您會在匯入執行時看到通知，並在匯入完成時看到最終結果。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   耶！

>[!NOTE]
>
>**相關文章**
>
>* [瞭解Marketo自訂物件](understanding-marketo-custom-objects.md)

>



