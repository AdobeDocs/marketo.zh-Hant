---
unique-page-id: 6848782
description: 將取消訂閱的訊息設為語言的動態訊息 — Marketo檔案 — 產品檔案
title: 讓您的取消訂閱訊息成為語言的動態訊息
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# 讓您的取消訂閱訊息成為語言的動態訊息 {#make-your-unsubscribe-message-dynamic-for-languages}

預設的取消訂閱訊息和連結為英文。 您可以使用動態內容以不同語言顯示。

>[!NOTE]
>
>本文代表最佳實務，但可以用其他方式完成。

## 準備您的資料 {#prepare-your-data}

1. [建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) 命名為「偏好的語言」。 （如果您想要同步此欄位，請在CRM中設定）。

   >[!TIP]
   >
   >將來，當您在下列情況下使用此欄位： [建立表單](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) 以擷取語言偏好設定。

## 建立細分 {#create-segmentation}

1. 前往 **[!UICONTROL 資料庫]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. 在 **[!UICONTROL 新增]** 下拉式清單，按一下 **[!UICONTROL 新區段]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. 為區段命名 **[!UICONTROL 偏好語言]**. 按一下 **[!UICONTROL 新增區段]**. 輸入語言。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >預設區段將為英文。

1. 繼續新增區段，直到所有語言皆有呈現為止。 按一下 **[!UICONTROL 建立]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. 選取區段。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. 前往 **[!UICONTROL 智慧清單]** 標籤。 輸入 **[!UICONTROL 偏好語言]** 至搜尋欄位。 將篩選器拖放至畫布上。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. 設定適當的對應語言。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. 對所有不同的語言重複此步驟。 然後，選取 **[!UICONTROL 分段動作]** 下拉式清單，然後按一下 **[!UICONTROL 核准]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## 建立代碼片段 {#create-a-snippet}

1. 前往 **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. 在 **[!UICONTROL 新增]** 下拉式清單，按一下 **[!UICONTROL 新增代碼片段]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. 為程式碼片段命名 **取消訂閱訊息**. 按一下 **[!UICONTROL 建立]**。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. 輸入預設的取消訂閱訊息，反白標示該訊息，然後按一下超連結圖示。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. 複製並貼上此Token： `{{system.unsubscribeLink}}` 到 **[!UICONTROL URL]** 欄位。 按一下 **[!UICONTROL 插入]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. 選取 **[!UICONTROL 區段依據]** 在 **[!UICONTROL 細分]** 區段。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. 從 **[!UICONTROL 細分]** 下拉式清單，輸入 **[!UICONTROL 偏好]** 並選取 **[!UICONTROL 偏好語言]**. 按一下 **[!UICONTROL 儲存]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. 從樹狀結構中選取區段。 按一下取消訂閱，然後按一下連結圖示。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. 確定 `{{system.unsubscribeLink}}` 仍在 **[!UICONTROL URL]** 欄位。 編輯 **[!UICONTROL 顯示文字]** 以符合您選取的語言。 按一下 **[!UICONTROL 套用]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. 對所有區段重複此步驟。 然後，返回 **[!UICONTROL Design Studio]**，按一下 **[!UICONTROL 程式碼片段動作]** 下拉式清單，然後按一下 **[!UICONTROL 核准]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

太棒了。 即將完成！

## 在電子郵件中使用程式碼片段 {#use-snippet-in-an-email}

1. 在電子郵件編輯器中，按一下可編輯的元素。 然後按一下齒輪圖示並選取 **[!UICONTROL 取代為代碼片段]**. 如果您選取的是可編輯的程式碼片段元素，請按一下齒輪圖示並選取 **[!UICONTROL 編輯]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. 從下拉式清單中尋找並選取您的程式碼片段，然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. 若要測試，請按一下 **[!UICONTROL 返回]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...然後 **[!UICONTROL 動態]** 標籤。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. 按一下不同的語言以檢視代碼片段變更。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >當然，您也可以編輯其他電子郵件的動態語言。 在您執行此操作時，請在取消訂閱頁面上執行相同的技巧。

## 使用動態內容自訂您的取消訂閱頁面 {#customizing-your-unsubscribe-page-with-dynamic-content}

如果您希望您的人員使用他們偏好的語言來進入取消訂閱頁面，您可以在登入頁面和確認頁面上使用動態內容。

1. 導覽至 **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. 輸入 _取消訂閱_ 在搜尋欄位中，並選取所需的「取消訂閱」頁面。

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. 按一下 **[!UICONTROL 編輯草稿]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. 選取 **[!UICONTROL 區段依據]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. 尋找 **[!UICONTROL 偏好語言]** 區段。 按一下 **[!UICONTROL 儲存]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   編輯每個登入頁面的內容、核准，一切準備就緒！

   >[!NOTE]
   >
   >進一步瞭解 [動態內容](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) 以及所有您能做的酷事。
