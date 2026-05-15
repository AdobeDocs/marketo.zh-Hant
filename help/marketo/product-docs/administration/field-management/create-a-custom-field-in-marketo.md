---
unique-page-id: 2360287
description: 在Marketo Engage中建立新自訂欄位以儲存和擷取人員或公司資料的步驟。
title: 在 Marketo 中建立自訂欄位
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
TQID: https://experienceleague.adobe.com/xdG07VzIcNYcqCsR3wfXHTGE07nsLYAvbM8QZZJf0oo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 191
ht-degree: 14%

---

# 在 Marketo 中建立自訂欄位 {#create-a-custom-field-in-marketo}

瞭解如何在Marketo Engage中建立自訂欄位以儲存和擷取資料。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. 按一下「**[!UICONTROL Field Management]**」。

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >如果您希望欄位與CRM保持同步，請在CRM中建立欄位，系統會自動在Marketo中建立這些欄位。

1. 按一下「**[!UICONTROL New Custom Field]**」。

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. 選擇&#x200B;_[!UICONTROL Object]_。

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >雖然您無法自行選取&#x200B;_公司_&#x200B;物件，但您可以聯絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}來要求它。

1. 選擇欄位&#x200B;_[!UICONTROL Type]_。 這會變更其在Marketo智慧清單和表單中的呈現方式。

   >[!TIP]
   >
   >請檢視[自訂欄位型別字彙表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}。

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. 輸入&#x200B;_[!UICONTROL Name]_，讓它在Marketo中顯示（會自動產生&#x200B;_[!UICONTROL API Name]_）。 請謹慎選擇，因為儲存後無法重新命名。 完成後請按一下 **[!UICONTROL Create]**。

>[!CAUTION]
>
>欄位名稱不能以下列字元開頭： **。 &amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>此API名稱會用於SOAP API和其他後端程式。

您現在可以在表單、流程步驟和智慧列示中使用此自訂欄位。
