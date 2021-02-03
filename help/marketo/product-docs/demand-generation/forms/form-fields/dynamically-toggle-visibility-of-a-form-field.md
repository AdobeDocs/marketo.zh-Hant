---
unique-page-id: 2949962
description: 動態切換表單欄位的可見性——行銷人員檔案——產品檔案
title: 動態切換表單欄位的可見性
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# 動態切換表單欄位{#dynamically-toggle-visibility-of-a-form-field}的可見性

>[!PREREQUISITES]
>
>* [新增國家／地區選取清單至表單](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Marketo表單最酷的功能之一，就是您可以動態隱藏／顯示表單欄位或[欄位集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md)。

>[!NOTE]
>
>**範例**
>
>在此範例中，讓我們隱藏&#x200B;**State**&#x200B;欄位，除非&#x200B;**Country**&#x200B;被選為&quot;United States&quot;。

1. 前往&#x200B;**行銷活動**。

   ![](assets/login-marketing-activities-8.png)

1. 選擇表單並按一下「編輯表單」。****

   ![](assets/editform-1.png)

1. 選擇要動態隱藏／顯示的欄位，然後按一下&#x200B;**可見性規則**&#x200B;的連結。

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 尋找並選取您要建立條件的欄位。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 選取運算子。

   >[!TIP]
   >
   >這很酷，因為您可以選擇模糊的比對，例如「開頭為」。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 選取要尋找的值，然後按一下下拉式清單外部。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >您可以在下拉式清單開啟時按一下多個值，以選取這些值。 例如，您可以選取「美國」和「加拿大」。

   >[!NOTE]
   >
   >我們先前將「國家／地區」轉換為挑選清單欄位類型，並且[新增所有國家／地區為值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)。

1. 按一下&#x200B;**保存**。

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就這樣！ 現在，當人們填妥此表單並選取「國家／地區的美國」時，「州」欄位會動態顯示指定的選項。
