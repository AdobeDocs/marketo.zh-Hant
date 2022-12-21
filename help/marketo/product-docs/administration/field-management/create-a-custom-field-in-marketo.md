---
unique-page-id: 2360287
description: 在Marketo中建立自訂欄位 — Marketo檔案 — 產品檔案
title: 在Marketo中建立自訂欄位
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 在Marketo中建立自訂欄位 {#create-a-custom-field-in-marketo}

如果您在Marketo中需要新的自訂欄位來儲存/擷取資料，以下說明如何建立資料。

1. 前往「管理」 ，然後按一下 **欄位管理**.

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >如果您希望欄位與CRM保持同步，請在CRM中建立欄位，系統就會自動在Marketo中建立欄位。

1. 按一下 **新自訂欄位**.

   ![](assets/two.png)

1. 選擇欄位「類型」。 這將變更Marketo中智慧清單和表單的呈現方式。

   >[!TIP]
   >
   >查看 [自訂欄位類型字彙表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. 輸入您希望其顯示在Marketo中的名稱。 系統會自動產生API名稱。 您可以加以調整，但一旦設定，就無法重新命名。 按一下 **建立** 時才能使用。

>[!CAUTION]
>
>欄位名稱的開頭不能為下列字元： **.&amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>SOAP API和其他後端程式會使用API名稱。

您現在可以在表單、流程步驟和智慧清單中使用此自訂欄位！
