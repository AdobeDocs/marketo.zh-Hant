---
unique-page-id: 6848782
description: 讓您的取消訂閱訊息在語言——行銷檔案——產品檔案中具動態性
title: 讓您的取消訂閱訊息在語言上具動態性
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---


# 讓您的取消訂閱訊息在語言上具動態性 {#make-your-unsubscribe-message-dynamic-for-languages}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

預設的取消訂閱訊息和連結為英文。 您可以使用動態內容以不同的語言顯示內容。

>[!NOTE]
>
>我們為您設定了這個不錯的教學課程。 這是一個最佳實踐，但可以通過其他方式實現。

1. 準備資料
1. [建立名為「](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)首選語言」的自訂欄位。 （如果您想要此欄位同步，請在CRM中設定）。

   >[!TIP]
   >
   >未來，當您建立表單以擷取語言 [偏好設定時](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md) ，請使用此欄位。

1. 建立區段
1. 轉到數 **據庫**。** ![](assets/db.png)

   **

1. 在「新 **增** 」下拉式清單中，按一 **下「新區段」**。

   ![](assets/two.png)

1. 將區段命名為 **偏好語言**。 按一 **下新增區段**。 輸入語言。

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >預設區段為英文。

1. 繼續新增區段，直到您的所有語言都已呈現。 按一下 **建立**。

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. 選取區段。

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. 轉到「智慧 **清單」** 頁籤。 在搜 **尋欄位中輸入** 「偏好語言」。 將篩選拖放至畫布上。

   ![](assets/six.png)

1. 設定相應的語言。

   ![](assets/seven.png)

1. 請針對您的所有不同語言重複。 然後，選取「 **區段動作** 」下拉式清單，然後按一下「 **核准」**。

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. 建立程式碼片段
1. 前往 **Design Studio**。

   ![](assets/ds.png)

1. 在「新增 **」下拉式清** 單中，按一 **下「新增程式碼片段**」。

   ** ![](assets/ten.png)

   **

1. 將程式碼片段命 **名為「取消訂閱訊息**」。 按一下 **建立**。

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. 輸入預設的取消訂閱訊息，反白標示訊息，然後按一下超連結圖示。

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. 複製並貼上此Token: **`{{system.unsubscribeLink}}`** 至「連 **結URL** 」欄位。 按一 **下插入**。

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. 在「 **區段** 」區段中選取「區段依據」。

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. 從「區段」下拉式清單中，輸入「首選 **語言** 」並選 **取「首選語言」**。 按一下 **儲存**。

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. 從樹中選擇一個段。 輸入該語言的取消訂閱訊息。

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. 複製並貼上相同的Token: **`{{system.unsubscribeLink}}`** 至「連 **結URL** 」欄位。 按一 **下插入**。

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. 對所有區段重複此動作。 然後，返回Design Studio，按一下「 **Snippet Actions** 」下拉式清單，然後按一下「 **Approve**」。

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   太棒了。 快到了。

1. 在電子郵件中使用程式碼片段
1. 在電子郵件編輯器中，按一下可編輯的元素。 然後按一下齒輪圖示，並選取「以程式碼 **片段取代」**。 如果您要選取可編輯的程式碼片段元素，請按一下齒輪圖示並選取「編 **輯」**。

   ![](assets/4.1.png)

1. 從下拉式清單中尋找並選取您的程式碼片段，然後按一下「 **儲存**」。

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. 若要測試，請按一 **下**...

   ![](assets/4.3.png)

1. ...，然後是「 **動態** 」頁籤。

   ![](assets/4.4.png)

1. 按一下不同的語言，即可看到程式碼片段變更。

   ![](assets/4.5.png)

   >[!TIP]
   >
   >當然，您也可以編輯電子郵件的其他內容，以取得動態語言。 在您執行時，請在取消訂閱頁面上執行相同的技巧。

1. 使用動態內容自訂您的取消訂閱頁面

   如果您希望您的人員以他們偏好的語言來取消訂閱頁面，您可以在登陸頁面和確認頁面上使用動態內容。

   導覽至Design Studio。

   ![](assets/ds.png)

   在搜尋欄位中輸入「取消訂閱」。 您應該找到「取消訂閱」頁面。

   ![](assets/image2015-3-9-8-3a51-3a53.png)

   按一下「編輯草稿」。

   ![](assets/image2015-3-9-8-3a52-3a23.png)

   選取區段依據。

   ![](assets/image2015-3-9-8-3a52-3a57.png)

   尋找「偏好語言」區段。 按一下「儲存」。

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   編輯每個登陸頁面的內容、核准，您就可以開始了！

   >[!NOTE]
   >
   >**深入探討**
   >
   >
   >進一步了 [解動態內容](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) ，以及您可以做的所有酷炫工作。

