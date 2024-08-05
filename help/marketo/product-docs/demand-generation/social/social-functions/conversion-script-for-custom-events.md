---
unique-page-id: 2950561
description: 自定義事件的轉換文本 - Marketo 檔案 - 產品檔
title: 自訂事件的轉換腳本
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 1%

---

# 自訂事件的轉換腳本 {#conversion-script-for-custom-events}

您在建立轉介優惠時定義履行目標。 如果計入目標的操作是您自己的 Web 頁面 上的特定事件，您可以使用轉換腳本調用我們的 JavaScript API。

>[!IMPORTANT]
>
>2024 年 7 月 31 日，我們開始棄用此功能。 您將無法創建新資產。 現有資產將持續工作到 2025 年 1 月 31 日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 擷取轉換腳本 {#retrieve-the-conversion-script}

1. 在轉介 優惠方案 編輯者中，按兩下「 **產品/服務詳細資訊** 」，然後從實現目標下拉列表中選擇 **「客戶JavaScript事件** 」。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 複製灰色框中的頂部腳本，並將其放置在您的網頁上的標籤內 `<body>` 。 底部腳本放置在標籤內 `<header>` 。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >如果腳本發佈到非 Marketo 網站上，請記得複製並貼上這兩個腳本。

## 擷取載入程式腳本 {#retrieve-the-loader-script}

1. 從樹狀結構中選擇轉介 優惠方案，然後按兩下 **「轉接選件動作** 」和 **「內嵌Code**」。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 以滑鼠右鍵按一下&#x200B;**頁首代碼**，並將其插入您的網頁頁首。 然後對&#x200B;**主體代碼**&#x200B;執行相同操作。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 將腳本粘貼到網頁上 {#pasting-the-scripts-onto-your-webpage}

將轉換腳本文件貼上至 HTML 中的正文和頁首。 下一個，請將載入程序腳本放入 HTML 中的內文和页首。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 連接轉換腳本 {#connecting-the-conversion-script}

在這裡，您將編寫一個JavaScript函數，該函數使用要觸發目標完成的任何頁面元素的特定 HTML ID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此示例中，網頁上有一個ID為“#myButtonId”的按鈕。 按兩下該按鈕時，此人將被註冊為已完成目標。

棒！ 您的網站現在正透過 Marketo 擷取自定義社交促銷活動目標。

>[!MORELIKETHIS]
>
>* [指定反向連結選件的目標](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [建立反向連結選件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的網站上部署Social](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
