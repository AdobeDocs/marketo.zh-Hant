---
unique-page-id: 2360287
description: 在Marketo中建立自訂欄位 — Marketo檔案 — 產品檔案
title: 在Marketo中建立自訂欄位
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 在Marketo中建立自訂欄位 {#create-a-custom-field-in-marketo}

如果您在Marketo Engage中需要新的自訂欄位來儲存/擷取資料，以下說明如何建立自訂欄位。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. 按一下&#x200B;**[!UICONTROL 欄位管理]**。

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >如果您希望欄位與CRM保持同步，請在CRM中建立欄位，系統會自動在Marketo中建立這些欄位。

1. 按一下&#x200B;**[!UICONTROL 新增自訂欄位]**。

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. 選擇欄位型別。 這會變更其在Marketo中智慧型清單和表單中的呈現方式。

   >[!TIP]
   >
   >請檢視[自訂欄位型別字彙表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)。

   ![](assets/create-a-custom-field-in-marketo-4.png)

1. 輸入[!UICONTROL 名稱]，使其在Marketo中顯示。 [!UICONTROL API名稱]會自動產生。 您可以調整它，但一旦設定就無法重新命名。 完成時，按一下&#x200B;**[!UICONTROL 建立]**。

>[!CAUTION]
>
>欄位名稱不能以下列字元開頭： **. &amp; +[]**

![](assets/create-a-custom-field-in-marketo-5.png)

>[!NOTE]
>
>SOAP API和其他後端處理程式會使用API名稱。

您現在可以在表單、流程步驟和智慧列示中使用此自訂欄位！
