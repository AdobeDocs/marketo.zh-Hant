---
unique-page-id: 2950555
description: 編輯Facebook豐富貼文設定 — Marketo檔案 — 產品檔案
title: 編輯Facebook豐富貼文設定
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# 編輯Facebook豐富貼文設定 {#edit-facebook-rich-post-settings}

當使用者在Facebook上分享您時自訂貼文。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的銷售代表。

Marketo [社交應用](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) 可讓您的潛在客戶與其在社交網路(例如Facebook、Twitter等)上的連線共用您的登錄頁面。 Facebook OpenGraph標籤（OG標籤）可讓您指定要將來自登陸頁面的資訊納入Facebook貼文中。

## 選取豐富貼文選項 {#select-rich-post-options}

您可以指定要在Facebook豐富貼文中使用的頁面資訊類型，這些豐富貼文是由您從登陸頁面分享產生的。

1. 選擇 **Facebook訊息** 在 **YouTube** 影片或社交按鈕。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 從下列選項中選取Facebook訊息。

   * 新增靜態內容：選擇此選項可手動輸入標題、標題和說明。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 新增動態內容：您的社交應用程式可使用登陸頁面 `<TITLE>`, `<CAPTION>`，和 `<DESCRIPTION>` 標籤來填入您的豐富貼文。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >這些標籤應已存在於頁面來源中，但如需更多控制，您可以將特定Facebook OG標籤新增至您的登錄頁面。

   * 請勿新增豐富內容：將Facebook貼文從您的登錄頁面限制為僅限主要訊息和連結。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 新增Facebook OG標籤至登陸頁面 {#add-facebook-og-tags-to-a-landing-page}

若要從您的登陸頁面控制Facebook共用中將包含的頁面元素，您可以將標題、註解和說明的Facebook OG(Open Graph)標籤新增至您的登陸頁面。

1. 開啟包含您 **YouTube影片** 或社交按鈕。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   此 **登錄頁面設計工具** 在新視窗中開啟。

1. 選擇 **登錄頁面動作** > **編輯頁面中繼標籤**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 新增定義og:title、og:caption和og:description的HTML。 複製並貼上這些行並取代預留位置文字：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>新增OG標籤時，請留意使用正確的HTML語法。
