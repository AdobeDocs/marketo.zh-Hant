---
unique-page-id: 2950555
description: 編輯Facebook Rich Post設定 — Marketo檔案 — 產品檔案
title: 編輯Facebook Rich Post設定
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# 編輯Facebook Rich Post設定 {#edit-facebook-rich-post-settings}

當有人在Facebook上分享您時自訂貼文。

>[!AVAILABILITY]
>
>並非所有客戶都已購買此功能。 如需詳細資訊，請聯絡您的銷售代表。

Marketo [社交應用程式](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) 允許您的潛在客戶與其在Facebook、Twitter等社交網路上的連線共用您的登陸頁面。 facebook OpenGraph標籤（OG標籤）可讓您指定登陸頁面中的哪些資訊包含在Facebook貼文中。

## 選取Rich Post選項 {#select-rich-post-options}

您可以指定要在由登入頁面中的共用產生的Facebook豐富貼文中使用的頁面資訊型別。

1. 選取 **facebook訊息** 在的編輯器中 **YouTube** 視訊或社交按鈕。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 從下列Facebook訊息選項中選取。

   * 新增靜態內容：選取此選項即可手動輸入標題、註解和說明。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 新增動態內容：您的社交應用程式可以使用登陸頁面的 `<TITLE>`， `<CAPTION>`、和 `<DESCRIPTION>` 標籤以填入您的豐富貼文。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >這些應已存在於頁面來源中，但如需更多控制權，您可以將特定的Facebook OG標籤新增至登陸頁面。

   * 不要新增豐富的內容：將登陸頁面的Facebook貼文限製為只新增主要訊息和連結。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 將Facebook OG標籤新增至登陸頁面 {#add-facebook-og-tags-to-a-landing-page}

若要控制從登陸頁面包含在Facebook共用中的頁面元素，您可以為登陸頁面新增標題、註解和說明的Facebook OG (Open Graph)標籤。

1. 開啟包含下列專案的登入頁面： **YouTube影片** 或社交按鈕。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   此 **登陸頁面設計工具** 會在新視窗中開啟。

1. 選取 **登陸頁面動作** > **編輯頁面中繼標籤**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 新增定義og：title、og：caption和og：description的HTML。 複製並貼上這些行並取代預留位置文字：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>新增OG標籤時，請務必注意使用正確的HTML語法。
