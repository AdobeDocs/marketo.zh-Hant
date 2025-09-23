---
unique-page-id: 6848782
description: 語言動態顯示取消訂閱訊息 — Marketo檔案 — 產品檔案
title: 讓您的取消訂閱訊息使用不同語言動態顯示
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 6%

---

# 讓您的取消訂閱訊息使用不同語言動態顯示 {#make-your-unsubscribe-message-dynamic-for-languages}

預設的取消訂閱訊息和連結為英文。 您可以使用動態內容以不同語言顯示。

>[!NOTE]
>
>本文代表最佳實務，但可以用其他方式完成。

## 準備您的資料 {#prepare-your-data}

1. [建立名為「偏好語言」的自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。 （如果您想要同步此欄位，請在CRM中進行設定）。

   >[!TIP]
   >
   >日後當您[建立表單](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)以擷取語言偏好設定時，請使用此欄位。

## 建立細分 {#create-segmentation}

1. 移至&#x200B;**[!UICONTROL Database]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單中，按一下&#x200B;**[!UICONTROL New Segmentation]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. 為區段&#x200B;**[!UICONTROL Preferred Language]**&#x200B;命名。 按一下&#x200B;**[!UICONTROL Add Segment]**。 輸入語言。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >預設區段將為英文。

1. 繼續新增區段，直到所有語言皆有呈現為止。 按一下「**[!UICONTROL Create]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. 選取區段。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. 前往&#x200B;**[!UICONTROL Smart List]**&#x200B;標籤。 在搜尋欄位中輸入&#x200B;**[!UICONTROL Preferred Language]**。 將篩選器拖放至畫布上。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. 設定適當的對應語言。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. 對所有不同的語言重複此步驟。 接著，選取&#x200B;**[!UICONTROL Segmentation Actions]**&#x200B;下拉式清單，然後按一下&#x200B;**[!UICONTROL Approve]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## 建立程式碼片段 {#create-a-snippet}

1. 移至&#x200B;**[!UICONTROL Design Studio]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單中，按一下&#x200B;**[!UICONTROL New Snippet]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. 將程式碼片段命名為&#x200B;**取消訂閱訊息**。 按一下「**[!UICONTROL Create]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. 輸入預設的取消訂閱訊息，反白該訊息，然後按一下超連結圖示。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. 將這個Token： `{{system.unsubscribeLink}}`複製並貼到&#x200B;**[!UICONTROL URL]**&#x200B;欄位中。 按一下「**[!UICONTROL Insert]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. 在&#x200B;**[!UICONTROL Segment By]**&#x200B;區段中選取&#x200B;**[!UICONTROL Segmentation]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. 從&#x200B;**[!UICONTROL Segmentation]**&#x200B;下拉式清單中，輸入&#x200B;**[!UICONTROL Preferred]**&#x200B;並選取&#x200B;**[!UICONTROL Preferred Language]**。 按一下「**[!UICONTROL Save]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. 從樹狀結構中選取區段。 按一下您的取消訂閱，然後按一下連結圖示。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. 確定`{{system.unsubscribeLink}}`仍在&#x200B;**[!UICONTROL URL]**&#x200B;欄位中。 編輯&#x200B;**[!UICONTROL Display Text]**&#x200B;以符合您選取的語言。 按一下「**[!UICONTROL Apply]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. 對所有區段重複。 接著，返回&#x200B;**[!UICONTROL Design Studio]**，按一下&#x200B;**[!UICONTROL Snippet Actions]**&#x200B;下拉式清單，然後按一下&#x200B;**[!UICONTROL Approve]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

棒極了！ 即將完成！

## 在電子郵件中使用程式碼片段 {#use-snippet-in-an-email}

1. 在電子郵件編輯器中，按一下可編輯的元素。 然後按一下齒輪圖示並選取&#x200B;**[!UICONTROL Replace with Snippet]**。 如果您選取的是可編輯的程式碼片段元素，請按一下齒輪圖示並選取&#x200B;**[!UICONTROL Edit]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. 從下拉式清單中尋找並選取您的程式碼片段，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. 若要測試它，請按一下&#x200B;**[!UICONTROL Back]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...然後&#x200B;**[!UICONTROL Dynamic]**&#x200B;索引標籤。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. 按一下不同的語言以檢視程式碼片段變更。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >當然，您也可以針對動態語言編輯電子郵件的其餘部分。 在您執行此操作時，請在取消訂閱頁面上執行相同的技巧。

## 使用動態內容自訂您的取消訂閱頁面 {#customizing-your-unsubscribe-page-with-dynamic-content}

如果您希望您的人員以偏好語言進入取消訂閱頁面，您可以使用登入頁面和確認頁面上的動態內容。

1. 導覽至&#x200B;**[!UICONTROL Design Studio]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. 在搜尋欄位中輸入&#x200B;_取消訂閱_，然後選取您想要的[取消訂閱]頁面。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. 按一下「**[!UICONTROL Edit Draft]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. 選取「**[!UICONTROL Segment By]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. 尋找&#x200B;**[!UICONTROL Preferred Language]**&#x200B;區段。 按一下「**[!UICONTROL Save]**」。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   編輯每個登入頁面的內容、核准，一切準備就緒！

   >[!NOTE]
   >
   >深入瞭解[動態內容](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md)以及您可以做的所有有趣事。
