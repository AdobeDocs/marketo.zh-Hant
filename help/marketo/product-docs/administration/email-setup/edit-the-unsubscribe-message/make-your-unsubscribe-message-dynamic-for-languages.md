---
unique-page-id: 6848782
description: 讓您的取消訂閱訊息動態顯示語言-Marketo檔案——產品檔案
title: 讓您的取消訂閱訊息在語言上具動態性
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# 讓取消訂閱訊息在語言上變得動態{#make-your-unsubscribe-message-dynamic-for-languages}

預設的取消訂閱訊息和連結為英文。 您可以使用動態內容以不同的語言顯示內容。

>[!NOTE]
>
>我們為您設定了這個不錯的教學課程。 這是一個最佳實踐，但可以通過其他方式實現。

## 準備資料{#prepare-your-data}

1. [建立名為「](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) 首選語言」的自訂欄位。（如果您想要此欄位同步，請在CRM中設定）。

   >[!TIP]
   >
   >以後，當您[建立表單](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)以擷取語言偏好設定時，請使用此欄位。

## 建立區段{#create-segmentation}

1. 轉至&#x200B;**Database**。

   ![](assets/db.png)

1. 在&#x200B;**New**&#x200B;下拉式清單中，按一下&#x200B;**New Segmentation**。

   ![](assets/two.png)

1. 將區段命名為&#x200B;**偏好語言**。 按一下「新增區段」。 ****&#x200B;輸入語言。

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >預設區段為英文。

1. 繼續新增區段，直到您的所有語言都已呈現。 按一下&#x200B;**建立**。

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. 選取區段。

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. 轉到&#x200B;**智慧清單**&#x200B;頁籤。 在搜索欄位中輸入&#x200B;**首選語言**。 將篩選拖放至畫布上。

   ![](assets/six.png)

1. 設定相應的語言。

   ![](assets/seven.png)

1. 請針對您的所有不同語言重複。 然後，選擇「分段動作」下拉式清單，然後按一下「核准」。********

   ![](assets/image2015-3-9-8-3a39-3a36.png)

## 建立程式碼片段{#create-a-snippet}

1. 前往&#x200B;**Design Studio**。

   ![](assets/ds.png)

1. 在&#x200B;**New**&#x200B;下拉式清單中，按一下「New Snippet」（新增程式碼片段）。****

   ![](assets/ten.png)

1. 為程式碼片段命名為&#x200B;**取消訂閱訊息**。 按一下&#x200B;**建立**。

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. 輸入預設的取消訂閱訊息，反白標示訊息，然後按一下超連結圖示。

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. 複製並貼上此Token:`{{system.unsubscribeLink}}`放入&#x200B;**連結URL**&#x200B;欄位。 按一下&#x200B;**插入**。

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. 在「區段」區段中選取「區段依據」**。**

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. 從「分段」下拉式清單中，輸入&#x200B;**Preferred**，然後選取&#x200B;**Preferred Language**。 按一下&#x200B;**保存**。

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. 從樹中選擇一個段。 輸入該語言的取消訂閱訊息。

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. 複製並貼上相同的Token:`{{system.unsubscribeLink}}`放入&#x200B;**連結URL**&#x200B;欄位。 按一下&#x200B;**插入**。

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. 對所有區段重複此動作。 然後，返回Design Studio，按一下「程式碼片段動作」下拉式清單，然後按一下「核准」。********

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   太棒了。 快到了。

## 在電子郵件{#use-snippet-in-an-email}中使用程式碼片段

1. 在電子郵件編輯器中，按一下可編輯的元素。 然後按一下齒輪圖示並選取「取代為程式碼片段」(Replace with Snippet)**。**&#x200B;如果要選擇可編輯的代碼片段元素，請按一下齒輪表徵圖並選擇&#x200B;**編輯**。

   ![](assets/4.1.png)

1. 從下拉式清單中尋找並選取您的程式碼片段，然後按一下「儲存」。****

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. 要測試它，請按一下&#x200B;**Back**...

   ![](assets/4.3.png)

1. ...然後，選擇&#x200B;**Dynamic**&#x200B;標籤。

   ![](assets/4.4.png)

1. 按一下不同的語言，即可看到程式碼片段變更。

   ![](assets/4.5.png)

   >[!TIP]
   >
   >當然，您也可以編輯電子郵件的其他內容，以取得動態語言。 在您執行時，請在取消訂閱頁面上執行相同的技巧。

## 使用動態內容{#customizing-your-unsubscribe-page-with-dynamic-content}自訂取消訂閱頁面

如果您希望您的人員以他們偏好的語言來取消訂閱頁面，您可以在登陸頁面和確認頁面上使用動態內容。

1. 導覽至Design Studio。

   ![](assets/ds.png)

1. 在搜尋欄位中鍵入&#x200B;_取消訂閱_。 您應該找到「取消訂閱」頁面。

   ![](assets/image2015-3-9-8-3a51-3a53.png)

1. 按一下「編輯草稿&#x200B;**」。**

   ![](assets/image2015-3-9-8-3a52-3a23.png)

1. 選擇&#x200B;**分段依據**。

   ![](assets/image2015-3-9-8-3a52-3a57.png)

1. 尋找「偏好語言」區段。 按一下&#x200B;**保存**。

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   編輯每個登陸頁面的內容、核准，您就可以開始了！

   >[!NOTE]
   >
   >進一步瞭解[動態內容](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md)以及您可以做的所有酷炫功能。
