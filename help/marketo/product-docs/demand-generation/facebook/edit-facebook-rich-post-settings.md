---
unique-page-id: 2950555
description: 編輯Facebook Rich Post設定 — Marketo檔案 — 產品檔案
title: 編輯Facebook Rich Post設定
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 7a8f5146126d6e8a4902be9337eef4d51e108cf0
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# 編輯Facebook Rich Post設定 {#edit-facebook-rich-post-settings}

當有人在Facebook上分享您時，請自訂貼文。

>[!AVAILABILITY]
>
>並非所有Marketo Engage使用者都已購買此功能。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

Marketo _社交應用程式_&#x200B;可讓您的潛在客戶透過其在Facebook、Twitter等社交網路上的連線，共用您的登陸頁面。 Facebook OpenGraph標籤（OG標籤）可讓您指定要將登陸頁面中的哪些資訊包含在Facebook貼文中。

## 選取Rich Post選項 {#select-rich-post-options}

您可以指定要在由登入頁面中的分享所產生的Facebook Rich Posts中使用的頁面資訊型別。

1. 在編輯器中選取&#x200B;**YouTube**&#x200B;視訊或社交按鈕的&#x200B;**Facebook訊息**。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 從下列Facebook訊息選項中選取。

   * 新增靜態內容：選取此選項即可手動輸入標題、註解和說明。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 新增動態內容：您的社交應用程式可以使用登陸頁面的`<TITLE>`、`<CAPTION>`和`<DESCRIPTION>`標籤來填入您的豐富貼文。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >這些應該已存在於頁面來源中，但為了取得更多控制權，您可以新增特定Facebook OG標籤至您的登入頁面。

   * 不要新增豐富的內容：將Facebook文章從您的登陸頁面限製為僅限主要訊息和連結。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 將Facebook OG標籤新增至登陸頁面 {#add-facebook-og-tags-to-a-landing-page}

若要控制從登陸頁面包含在Facebook共用中的頁面元素，您可以為登陸頁面新增標題、標題和說明的Facebook OG （開放圖表）標籤。

1. 開啟包含您的&#x200B;**YouTube影片**&#x200B;或社交按鈕的登陸頁面。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **登陸頁面Designer**&#x200B;會在新視窗中開啟。

1. 選取&#x200B;**登陸頁面動作** > **編輯頁面中繼標籤**。

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 新增定義og：title、og：caption和og：description的HTML。 複製並貼上這些行並取代預留位置文字：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>新增OG標籤時，請務必使用正確的HTML語法。
