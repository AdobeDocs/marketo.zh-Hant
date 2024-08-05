---
unique-page-id: 2950524
description: 在您的網站上部署Social - Marketo 檔 - 產品檔
title: 在您的網站上部署Social
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 在您的網站上部署Social {#deploy-social-on-your-website}

在非 Marketo 頁面上內嵌社交應用程式。

>[!IMPORTANT]
>
>2024 年 7 月 31 日，我們開始棄用此功能。 您將無法創建新資產。 現有資產將持續工作到 2025 年 1 月 31 日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>並非所有Marketo Engage用戶都購買了此功能。 請洽詢 Adobe Systems 客戶團隊 （您的帳戶管理員） 以取得詳細資訊。

您可以在自己的網站上部署社交應用程式，以吸引您的對象並將每個人帶入社交網路上的更大對話。 當人們在社交網路上與他們的朋友分享您的促銷和內容時，您會在您的網站上產生更多流量。

1. 選取已核准的社交應用程式，例如 YouTube 影片或Social按鈕。

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. 從 **「動作Social 應用程式選取「內嵌Code** 」。

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. 複製您網站頁面標題 （`<head>`） 和內文 （`<body>`） 的程序代碼。

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. 將第一個代碼段貼上至網站的 頁面 標頭。

   ![](assets/socialonsite-embedhead.png)

1. 將第二個代碼段貼上到您希望社交應用出現在頁面中的每個頁面。

   ![](assets/socialonsite-embedwidget.png)

1. 如果您需要在頁面上將社交應用的大小設置為特定尺寸，請將 outerHeight **和** outerWidth **選項添加到**&#x200B;第二個代碼段。例如，您可以添加 `options='{"outerHeight":400, "outerWidth":600}'`，如：

   ![](assets/socialonsite-resizewidget2.png)

   您的 Marketo 社交應用程式現在為您的網站添加了內容和互動，邀請粉絲、訪問者和現有客戶來宣傳您。 同時，它將他們的設定檔數據添加到您的資料庫中並跟蹤社交影響力指標。

   >[!MORELIKETHIS]
   >
   >* [自訂Social 應用程式按鈕](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [設定Social份額要求](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish登陸頁面至 Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
