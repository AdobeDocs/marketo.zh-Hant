---
unique-page-id: 2950555
description: 編輯Facebook豐富型貼文設定——行銷檔案——產品檔案
title: 編輯Facebook豐富型貼文設定
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---


# 編輯Facebook豐富型貼文設定{#edit-facebook-rich-post-settings}

當人們在Facebook上分享您時，自訂貼文。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請洽詢您的銷售代表。

Marketo [社交應用程式](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md)可讓您的潛在客戶在社交網路（例如Facebook、Twitter等）上與其連線共用您的登陸頁面。 Facebook OpenGraph標籤（OG標籤）可讓您指定Facebook貼文中包含著陸頁面的資訊。

## 選取豐富式貼文選項{#select-rich-post-options}

您可以指定要在來自著陸頁面的分享所產生的Facebook豐富型貼文中使用的頁面資訊類型。

1. 在編輯器中為您的&#x200B;**YouTube**&#x200B;影片或社交按鈕選擇&#x200B;**Facebook訊息**。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 從下列選項中選取您的Facebook訊息。

   * 新增靜態內容：選擇此選項可手動輸入標題、標題和說明。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 新增動態內容：您的社交應用程式可以使用登陸頁面的`<TITLE>`、`<CAPTION>`和`<DESCRIPTION>`標籤來填入您的豐富貼文。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >這些標籤應已存在於頁面來源中，但若要進一步控制，您可以將特定Facebook OG標籤新增至著陸頁面。

   * 不要新增多樣化內容：將登陸頁面的Facebook貼文限制為主要訊息和連結。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 新增Facebook OG標籤至著陸頁面{#add-facebook-og-tags-to-a-landing-page}

若要控制來自著陸頁面的Facebook分享中將包含的頁面元素，您可以將標題、標題和說明的Facebook OG(Open Graph)標籤新增至著陸頁面。

1. 開啟包含&#x200B;**YouTube影片**&#x200B;或社交按鈕的著陸頁面。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **著陸頁面設計器**&#x200B;會在新視窗中開啟。

1. 選擇「**著陸頁面動作** > **編輯頁面中繼標籤**」。

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 新增定義og:title、og:caption和og:description的HTML。 複製並貼上這些行並取代預留位置文字：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>新增OG標籤時，請務必使用正確的HTML語法。
