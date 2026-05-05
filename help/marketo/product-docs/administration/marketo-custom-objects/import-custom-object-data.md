---
unique-page-id: 10099680
description: 使用CSV檔案匯入自訂物件資料的步驟，包括選取自訂物件、重複資料刪除模式，以及欄位對應。
title: 匯入自訂物件資料
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 40d7e8a0723946970c49a6dfc4f0de4c71b0df65
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 4%

---

# 匯入自訂物件資料 {#import-custom-object-data}

請依照下列步驟，將自訂物件資料匯入資料庫。 若您正在使用公司自訂物件，請參閱[使用公司自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies)以取得詳細資訊。

1. 在「我的Marketo」中，移至&#x200B;**[!UICONTROL Database]**。

   ![](assets/import-custom-object-data-1.png)

1. 按一下&#x200B;**[!UICONTROL New]**&#x200B;並選取&#x200B;**[!UICONTROL Import Custom Object Data]**。

   ![](assets/import-custom-object-data-2.png)

1. 按一下&#x200B;**[!UICONTROL Browse]**&#x200B;以尋找資料檔。 選取檔案格式（在此範例中為逗號分隔值）。

   ![](assets/import-custom-object-data-3.png)

1. 選取您的[!UICONTROL custom object]。

   ![](assets/import-custom-object-data-4.png)

1. 從下拉式清單中選取[!UICONTROL Dedupe Mode]。 按一下「**[!UICONTROL Next]**」。

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >當您建立或更新自訂物件記錄時，請使用一或多個重複資料刪除欄位做為唯一識別碼。 此範例使用&#x200B;**car**&#x200B;自訂物件 — vin （車輛識別碼）的重複資料刪除欄位。 如果您只更新自訂物件記錄，則可以選取[!UICONTROL Marketo Guid]作為[!UICONTROL Dedupe Mode]。

1. 將每一欄對應至Marketo欄位，從下拉式清單中選取它。

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >確保檔案中的值與您比對的欄位型別相符（例如文字、整數等），否則檔案將被拒絕。

1. 按一下「**[!UICONTROL Next]**」。

   ![](assets/import-custom-object-data-7.png)

1. 按一下「**[!UICONTROL Import]**」。

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >自訂物件的大小限製為100MB。

   >[!TIP]
   >
   >在「**[!UICONTROL Send Alert To]**」欄位中輸入您的電子郵件地址，Marketo將在匯入完成時以電子郵件通知您。

1. 在熒幕右上角，您會在匯入執行時看到通知，並在匯入完成時看到最終結果。

   ![](assets/import-custom-object-data-9.png)

>[!MORELIKETHIS]
>
>[瞭解Marketo自訂物件](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
