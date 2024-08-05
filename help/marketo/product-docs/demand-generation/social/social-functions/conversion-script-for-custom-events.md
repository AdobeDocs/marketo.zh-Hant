---
unique-page-id: 2950561
description: 自訂事件的轉換指令碼 — Marketo檔案 — 產品檔案
title: 自訂事件的轉換指令碼
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# 自訂事件的轉換指令碼 {#conversion-script-for-custom-events}

您在建立轉介優惠時定義履行目標。 如果計入目標的動作是您網頁上的特定事件，則您可以使用轉換指令碼來呼叫JavaScript API。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 無法再建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 擷取轉換指令碼 {#retrieve-the-conversion-script}

1. 在轉介優惠編輯器中，按一下&#x200B;**優惠詳細資料**，然後從履行目標下拉式清單中選取&#x200B;**客戶JavaScript事件**。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 複製灰色方塊中的最上層指令碼，並將其放在網頁的`<body>`標籤內。 底部指令碼置於`<header>`標籤內。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >如果指令碼在非Marketo網站上運作，請記得複製並貼上這兩個指令碼。

## 擷取載入器指令碼 {#retrieve-the-loader-script}

1. 從樹狀結構選取轉介選件，然後按一下&#x200B;**轉介選件動作**&#x200B;和&#x200B;**內嵌程式碼**。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 以滑鼠右鍵按一下&#x200B;**頁首代碼**，並將其插入您的網頁頁首。 然後對&#x200B;**主體代碼**&#x200B;執行相同操作。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 將指令碼貼到網頁上 {#pasting-the-scripts-onto-your-webpage}

將轉換指令碼貼到內文和標題的HTML中。 接著，將載入器指令碼放入內文和標題的HTML中。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 連線轉換指令碼 {#connecting-the-conversion-script}

您將在此處撰寫JavaScript函式，此函式會使用您要觸發目標完成之任何頁面元素的特定HTMLID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此範例中，網頁上有一個識別碼為「#myButtonId」的按鈕。 按一下該按鈕時，該人員將註冊為已完成目標。

棒極了！ 您的網站現在正透過Marketo擷取自訂社交促銷活動的目標。

>[!MORELIKETHIS]
>
>* [指定轉介選件的目標](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [建立轉介選件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的網站上部署Social](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
