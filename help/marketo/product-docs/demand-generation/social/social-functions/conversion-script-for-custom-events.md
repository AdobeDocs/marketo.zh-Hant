---
unique-page-id: 2950561
description: 自訂事件的轉換指令碼 — Marketo檔案 — 產品檔案
title: 自訂事件的轉換指令碼
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# 自訂事件的轉換指令碼 {#conversion-script-for-custom-events}

您在建立轉介優惠時定義履行目標。 如果計入目標的動作是您網頁上的特定事件，則您可以使用轉換指令碼來呼叫JavaScript API。

## 擷取轉換指令碼 {#retrieve-the-conversion-script}

1. 在推薦選件編輯器中，按一下 **優惠詳細資料** 然後選取 **客戶JavaScript事件** 「達成目標」下拉式清單。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 複製灰色方塊中的頂端指令碼，並將其放置在網頁內的 `<body>` 標籤之間。 底部指令碼會置於 `<header>` 標籤之間。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >如果指令碼在非Marketo網站上運作，請記得複製並貼上這兩個指令碼。

## 擷取載入器指令碼 {#retrieve-the-loader-script}

1. 從樹狀結構中選取反向連結選件，然後按一下 **反向連結優惠動作** 和 **內嵌程式碼**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 用滑鼠右鍵按一下 **頁首程式碼** 並將其插入網頁標題。 然後對 **內文**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 將指令碼貼到網頁上 {#pasting-the-scripts-onto-your-webpage}

將轉換指令碼貼到內文和標題的HTML中。 接著，將載入器指令碼放入內文和標題的HTML中。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 連線轉換指令碼 {#connecting-the-conversion-script}

您可以在此處撰寫JavaScript函式，此函式會使用您要觸發目標完成之任何頁面元素的特定HTMLID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此範例中，網頁上有一個識別碼為「#myButtonId」的按鈕。 按一下該按鈕時，該人員將註冊為已完成目標。

棒極了！ 您的網站現在正透過Marketo擷取自訂社交促銷活動的目標。

>[!MORELIKETHIS]
>
>* [指定轉介優惠的目標](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [建立反向連結選件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的網站上部署Social](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
