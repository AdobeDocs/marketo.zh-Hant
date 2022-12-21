---
unique-page-id: 10099680
description: 匯入自訂物件資料 — Marketo檔案 — 產品檔案
title: 匯入自訂物件資料
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 匯入自訂物件資料 {#import-custom-object-data}

將自訂物件資料匯入資料庫相當容易。 如果您正在公司中使用自訂物件，請參閱 [搭配公司使用自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) 以取得更多資訊。

1. 在我的Marketo中，前往 **資料庫**.

   ![](assets/db-1.png)

1. 按一下 **新增** 選取 **匯入自訂物件資料**.

   ![](assets/image2016-4-7-10-6-54.png)

1. 按一下 **瀏覽** 來尋找資料檔案。 選取檔案格式（此範例中為逗號分隔值）。

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. 選取自訂物件。

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. 從下拉清單中選擇重複資料消除模式。 按一下 **下一個**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >建立或更新自定義對象記錄時，請使用重複資料消除欄位作為唯一標識符。 此示例使用 **汽車** 自訂物件 — vin（車輛ID號碼）。 如果只更新自定義對象記錄，則可以選擇「Marketo Guid」作為重複資料刪除模式。

1. 將每欄對應至Marketo欄位，從下拉式清單中選取欄位。

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >請確定檔案中的值與您要比對的欄位類型相符（例如文字、整數等），否則檔案將遭拒。

1. 按一下 **下一個**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. 按一下 **匯入**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >自訂物件的大小限制為100MB。

   >[!TIP]
   >
   >在 **將警報發送到：** 欄位和Marketo會在您完成匯入時傳送電子郵件給您！

1. 在畫面的右上角，您會在匯入執行時看到通知，並在匯入完成時看到最終結果。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   耶！

>[!MORELIKETHIS]
>
>[了解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
