---
unique-page-id: 2950549
description: 設定社交建議流程 — Marketo檔案 — 產品檔案
title: 設定社交建議流量
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 設定社交建議流量 {#configure-social-recommend-flow}

當您建立社交應用程式時，可以設定社交網路選擇，並提示使用者在註冊時遇到。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 無法再建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 選取要共用的網路 {#select-networks-for-sharing}

>[!NOTE]
>
>這非常類似於[設定社交註冊/共用流程](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md)，但這適用於社交應用程式&#x200B;_下的共用連結_。

1. 移至&#x200B;**行銷活動**。

   ![](assets/login-marketing-activities-1.png)

1. 選取應用程式，然後按一下&#x200B;**編輯草稿**。

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. 在社交應用程式編輯器中，移至&#x200B;**建議流量** > **社交網路**。

   ![](assets/recommendedflow.png)

1. 選取使用者可以分享的網路。

   ![](assets/socialnetworkschoose.png)

## 設定Facebook訊息 {#configure-the-facebook-message}

1. 設定將顯示在Facebook貼文中的訊息。

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >在視訊共用中，縮圖會自動產生。

   如果您選擇&#x200B;**新增動態內容**，頁面的OpenGraph標籤（og：title、og：caption和og：description）和縮圖的值會自動新增到Facebook貼文中。 請參閱下一步。

   如果您選擇&#x200B;**新增靜態內容**，請輸入標題、標題和說明，然後上傳影像。 請參閱接下來的兩個步驟。

1. 在[檢視與編輯]視窗中，按一下[顯示編輯專案] ****&#x200B;以自訂將在Facebook文章中顯示的共用提示與訊息。

   >[!TIP]
   >
   >如需詳細資訊，請參閱[編輯Facebook豐富貼文設定](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md)。

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >[共用URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)會自動新增至所有共用訊息。

1. 如果您選擇上述&#x200B;**新增靜態內容**，請編輯標題、標題和說明，並上傳自訂影像(從您的Marketo影像和檔案)。

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   請參閱[將影像和檔案新增至Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)。

   >[!NOTE]
   >
   >如果您上傳影像，在關閉並重新開啟社交應用程式編輯器之前，您不會在這裡看到影像。

1. 按一下&#x200B;**下一步**。

如果選擇「 」，則頁面OpenGraph標籤的值（og：title、og：caption和og：description）和縮圖會自動新增到Facebook貼文中。 請參閱下一步。

## 設定Twitter訊息 {#configure-the-twitter-message}

1. 按一下以編輯分享提示和將顯示在Twitter推文中的訊息。

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >在推文文字中使用{html_title}自動顯示頁面標題。

1. 按一下&#x200B;**下一步**。

## 設定LinkedIn訊息 {#configure-the-linkedin-message}

1. 設定將顯示在LinkedIn貼文中的訊息。

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   如果您選擇&#x200B;**新增動態**&#x200B;內容，頁面標籤的值（標題和說明）以及縮圖會自動新增到LinkedIn貼文。 請參閱下一步。

   如果您選擇&#x200B;**新增靜態**&#x200B;內容，請輸入標題、標題和說明，然後上傳影像。 請參閱接下來的兩個步驟。

1. 在&#x200B;**檢視和編輯**&#x200B;視窗中，按一下&#x200B;**顯示編輯專案**，並編輯將在LinkedIn文章中顯示的共用提示和訊息。

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >在您的文章文字中使用{html_title}自動顯示頁面標題。

1. 如果您選擇上述&#x200B;**新增靜態**&#x200B;內容，請編輯標題和說明，並上傳自訂影像(從您的Marketo影像和檔案)。

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   請參閱[將影像和檔案新增至Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)。

   >[!NOTE]
   >
   >如果您上傳影像，在關閉並重新開啟社交應用程式編輯器之前，您不會在這裡看到影像。

1. 按一下&#x200B;**下一步**。

## 設定確認訊息 {#configure-the-confirmation-message}

1. 編輯共用確認文字。

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. 按一下&#x200B;**完成** > **核准**&#x200B;和&#x200B;**關閉**。

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>下一步是[將您的視訊共用](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md)或[輪詢](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md)新增至登陸頁面、Facebook或您自己的網站。
