---
unique-page-id: 2949962
description: 動態切換表單欄位的可見度 — Marketo檔案 — 產品檔案
title: 動態切換表單欄位的可見度
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 動態切換表單欄位的可見度 {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [新增國家/地區選擇清單至您的表單](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Marketo表單的一個真正酷的功能是您可以動態隱藏/顯示表單欄位或 [欄位集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**範例**
>
>在此範例中，讓我們隱藏 **州** 欄位，除非 **國家** 被選為「美國」。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-8.png)

1. 選取您的表單並按一下 **編輯表單**.

   ![](assets/editform-1.png)

1. 選取您要動態隱藏/顯示的欄位，然後按一下連結 **可見度規則**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 尋找並選取您要建立條件的欄位。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 選取運運算元。

   >[!TIP]
   >
   >這很酷，因為您可以選擇模糊的相符專案，例如「開頭為」。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 選取要尋找的值，然後在下拉式清單外部按一下。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >您可以在下拉式清單開啟時按一下多個值，以選取多個值。 例如，您可以選取「美國」和「加拿大」。

   >[!NOTE]
   >
   >我們先前將「國家/地區」轉換為挑選清單欄位型別，並且 [將所有國家/地區新增為值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. 按一下 **儲存**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就是這樣！ 現在，當人們填寫此表單並選取「美國國家/地區」時，「州」欄位將會以指定的選項動態顯示。

>[!IMPORTANT]
>
>透過自訂指令碼使用設定/更新欄位值時，表單欄位行為將順暢運作 [API函式](https://developers.marketo.com/javascript-api/forms/){target="_blank"} 在Forms 2.0中。
>
>如果欄位值由Forms 2.0 JavaScript API以外的外部指令碼修改，則條件欄位可能無法如預期運作。
