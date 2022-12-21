---
unique-page-id: 2950561
description: 自訂事件的轉換指令碼 — Marketo檔案 — 產品檔案
title: 自訂事件的轉換指令碼
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# 自訂事件的轉換指令碼 {#conversion-script-for-custom-events}

建立轉介優惠方案時，您會定義完成目標。 如果對目標計數的動作是您自己網頁上的特定事件，您可以使用轉換指令碼來呼叫我們的JavaScript API。

## 擷取轉換指令碼 {#retrieve-the-conversion-script}

1. 在反向連結選件編輯器中，按一下 **優惠方案詳細資訊** 然後選取 **客戶JavaScript事件** 完成目標下拉式清單中。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 複製灰色方塊中的頂端指令碼，並將其放置在 `<body>` 標籤。 底部指令碼放在 `<header>` 標籤。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >如果兩個指令碼正在非Marketo網站上，請記得複製並貼上。

## 檢索載入器指令碼 {#retrieve-the-loader-script}

1. 從樹狀結構中選取反向連結選件，然後按一下 **轉介選件動作** 和 **內嵌程式碼**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 以滑鼠右鍵按一下 **標題代碼** 並插入網頁標題。 然後對 **內文程式碼**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 將指令碼貼到您的網頁上 {#pasting-the-scripts-onto-your-webpage}

將轉換指令碼貼入內文和標題的HTML中。 接下來，將載入器指令碼放入主體和標頭的HTML中。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 連接轉換指令碼 {#connecting-the-conversion-script}

以下是您要編寫JavaScript函式的位置，此函式會使用任何您要觸發目標完成的頁面元素的特定HTMLID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此範例中，網頁上有一個ID為「#myButtonId」的按鈕。 按一下該按鈕後，會將人員註冊為已完成目標。

太棒了！ 您的網站現在正使用Marketo擷取自訂的社交促銷目標。

>[!MORELIKETHIS]
>
>* [指定轉介選件的目標](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [建立反向連結選件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的網站上部署Social](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

