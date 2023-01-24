---
unique-page-id: 2949962
description: 動態切換表單欄位的可見性 — Marketo檔案 — 產品檔案
title: 動態切換表單欄位的可見性
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
source-git-commit: 0aa754bb3fb9057aaec87dc41743711fb15f8d62
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 動態切換表單欄位的可見性 {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [將國家/地區選擇清單添加到表單](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Marketo表單最酷的一項功能，是您可以動態隱藏/顯示表單欄位或 [欄位集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**範例**
>
>在此範例中，我們將隱藏 **狀態** 除非 **國家/地區** 被選為「美國」。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-8.png)

1. 選取您的表單並按一下 **編輯表單**.

   ![](assets/editform-1.png)

1. 選取您要動態隱藏/顯示的欄位，然後按一下的連結 **可見性規則**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 尋找並選取要建立條件的欄位。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 選取運算子。

   >[!TIP]
   >
   >這很酷，因為您可以選取模糊比對，例如「開頭為」。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 選取要尋找的值，然後按一下下拉式清單外部的。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >您可以在下拉式清單開啟時按一下多個值，以選取這些值。 例如，您可以選取「美國」和「加拿大」。

   >[!NOTE]
   >
   >我們先前將「國家/地區」轉換為挑庫清單欄位類型，並 [新增所有國家/地區為值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. 按一下 **儲存**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就這樣！ 現在，當人們填寫此表單並選擇「國家/地區的美國」時，「州」欄位將動態顯示並指定選項。

>[!IMPORTANT]
>
>透過使用的自訂指令碼設定/更新欄位值時，表單欄位行為將可順暢運作 [API函式](https://developers.marketo.com/javascript-api/forms/){target="_blank"} 在Forms 2.0中。
>
>如果欄位值是由Forms 2.0 JavaScript API以外的外部指令碼修改，條件欄位可能無法如預期運作。
