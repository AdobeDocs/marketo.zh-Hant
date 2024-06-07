---
unique-page-id: 2949962
description: 動態切換表單欄位的可見度 — Marketo檔案 — 產品檔案
title: 動態切換表單欄位的可見度
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 動態切換表單欄位的可見度 {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [新增國家/地區選擇清單至您的表單](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Marketo表單很酷的一個功能是您可以動態隱藏/顯示表單欄位或 [欄位集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**範例**
>
>在此範例中，讓我們隱藏 **狀態** 欄位除非 **國家** 被選為「美國」。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-8.png)

1. 選擇您的表單並按一下 **編輯表單**.

   ![](assets/editform-1.png)

1. 選取您要動態隱藏/顯示的欄位，然後按一下連結 **可見度規則**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 尋找並選取您要建立條件的欄位。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 選取運運算元。

   >[!TIP]
   >
   >這很酷，因為您可以選擇模糊的符合專案，例如「開頭為」。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 選取要尋找的值，然後按一下下拉式清單外部的。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >您可以在下拉式清單開啟時按一下多個值，以選取多個值。 例如，您可以選取「美國」和「加拿大」。

   >[!NOTE]
   >
   >我們先前將「國家/地區」轉換為挑選清單欄位型別並 [將所有國家/地區新增為值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. 按一下&#x200B;**保存**。

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就是這樣！ 現在，當人們填寫此表格並選取「美國國家」時，「州」欄位將會以指定的選項動態顯示。

>[!IMPORTANT]
>
>使用透過自訂指令碼設定/更新欄位值時，表單欄位行為將順暢運作 [API函式](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} 在Forms 2.0中。
>
>如果欄位值是由Forms 2.0 JavaScript API以外的外部指令碼修改，則條件欄位可能無法如預期運作。
