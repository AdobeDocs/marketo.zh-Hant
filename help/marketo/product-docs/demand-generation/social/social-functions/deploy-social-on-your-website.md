---
unique-page-id: 2950524
description: 在您的網站上部署Social - Marketo檔案 — 產品檔案
title: 在您的網站上部署Social
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 在您的網站上部署Social {#deploy-social-on-your-website}

在非Marketo頁面上內嵌社交應用程式。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 無法再建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>並非所有Marketo Engage使用者都已購買此功能。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

您可以在自己的網站上部署社交應用程式，以吸引觀眾參與，並讓每個人都參與社交網路上的大型對話。 當人們在社交網路上與好友分享您的促銷活動和內容時，您會在網站上產生更多流量。

1. 選取核准的社交應用程式，例如YouTube影片或社交按鈕。

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. 從社交應用程式動作中選取&#x200B;**內嵌程式碼**。

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. 複製網站頁首(`<head>`)和內文(`<body>`)的程式碼。

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. 將第一個程式碼片段貼入網站的頁首。

   ![](assets/socialonsite-embedhead.png)

1. 將第二個程式碼片段貼到每個頁面，讓您的社交應用程式顯示在該頁面上。

   ![](assets/socialonsite-embedwidget.png)

1. 如果您需要將社交應用程式的大小設定為頁面上的特定維度，請將&#x200B;**outerHeight**&#x200B;和&#x200B;**outerWidth**&#x200B;選項新增至第二個程式碼片段。 例如，您可以新增`options='{"outerHeight":400, "outerWidth":600}'`，如下所示：

   ![](assets/socialonsite-resizewidget2.png)

   您的Marketo社交應用程式現在新增內容與互動功能至您的網站，邀請粉絲、訪客和現有客戶傳播您的相關資訊。 同時，這會將他們的設定檔資料新增到您的資料庫，並追蹤社交影響力量度。

   >[!MORELIKETHIS]
   >
   >* [自訂社交應用程式按鈕](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [設定社交分享需求](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish登陸頁面至Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
