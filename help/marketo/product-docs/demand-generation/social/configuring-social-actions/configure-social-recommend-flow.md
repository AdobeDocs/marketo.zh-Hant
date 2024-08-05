---
unique-page-id: 2950549
description: 設定社交建議流程 — Marketo檔案 — 產品檔案
title: 設定社交建議流量
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 設定社交建議流量 {#configure-social-recommend-flow}

當您建立社交應用程式時，可以設定社交網路選擇，並提示使用者在註冊時遇到。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 您將無法建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 選取要共用的網路 {#select-networks-for-sharing}

>[!NOTE]
>
>這非常類似於[設定社交註冊/共用流程](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md)，但這適用於社交應用程式&#x200B;_下的共用連結_。

1. 移至&#x200B;**行銷活動**。

   ![](assets/login-marketing-activities-1.png)

1. 選取應用程式，然後按兩下 **「草稿**&#x200B;編輯」。

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. 在社交應用編輯者中，前往&#x200B;**「建議流量>****Social網路**」。

   ![](assets/recommendedflow.png)

1. 選擇用戶可以共享到的網路。

   ![](assets/socialnetworkschoose.png)

## 設定 Facebook 新增訊息 {#configure-the-facebook-message}

1. 設定將在 Facebook 貼文中顯示的訊息。

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >在視訊共用中，縮圖是自動生成的。

   如果您選擇 **添加動態內容**，頁面的 OpenGraph 標籤（og：title、og：caption 和 og：description）和縮略圖的值會自動添加到 Facebook 帖子中。 請參閱下一個步驟。

   如果您選擇 **「新增靜態內容**」，請輸入標題、題注和說明，然後上傳影像。 請參閱接下來的兩個步驟。

1. 在檢視和編輯窗口中，按兩下 **顯示** 编辑以自定義將在Facebook帖子中显示的共享提示和消息。

   >[!TIP]
   >
   >如需詳細信息，請参閱 [編輯 Facebook Rich Post 設定](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md)。

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

## 設定LinkedIn 新增訊息 {#configure-the-linkedin-message}

1. 設定要在LinkedIn帖子中顯示的訊息。

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   如果您選擇添加 **動態** 內容，則頁面標記（標題和說明）和縮略圖的值將自動添加到LinkedIn帖子中。 請參閱下一個步驟。

   如果您選擇 **「新增靜態** 內容」，請輸入標題、題注和說明，然後上傳影像。 請參閱接下來的兩個步驟。

1. 在 **檢視和編輯** 窗口中，按兩下 **顯示** 编辑並編輯將在LinkedIn帖子中显示的共享提示和消息。

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >在貼文文字中使用 {html_title} ，以自動顯示頁面標題。

1. 如果您在上面選擇了 **添加靜態** 內容，請編輯標題和說明，然後上傳自定義映像（來自 Marketo 映射和檔案）。

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   請參閱 [向 Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md) 添加映像和檔案。

   >[!NOTE]
   >
   >如果您上傳圖片，則在關閉並重新打開社交應用編輯者之前，您不會在此處看到該圖片。

1. 按兩下一個&#x200B;****。

## 設定確認訊息 {#configure-the-confirmation-message}

1. 編輯共用確認文字。

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. 按一下&#x200B;**完成** > **核准**&#x200B;和&#x200B;**關閉**。

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>下一步是[將您的視訊共用](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md)或[輪詢](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md)新增至登陸頁面、Facebook或您自己的網站。
