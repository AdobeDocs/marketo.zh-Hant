---
unique-page-id: 2950561
description: 自訂事件的轉換指令碼——行銷人員檔案——產品檔案
title: 自訂事件的轉換指令碼
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# 自訂事件的轉換指令碼 {#conversion-script-for-custom-events}

您可在建立反向連結選件時定義履約目標。 如果針對目標的動作是您自己網頁上的特定事件，您可以使用轉換指令碼來呼叫我們的JavaScript API。

## 擷取轉換指令碼 {#retrieve-the-conversion-script}

1. 在反向連結選件編輯器中，按一 **下選件詳細資訊** ，然後從履約目標下拉式清 **單中選取「客戶JavaScript事件** 」。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 複製灰色方塊中的頂端指令碼，並將它放置在您的網頁上的標 `<body>` 簽中。 底部指令檔會放在標籤 `<header>` 中。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果指令檔正在非Marketo網站上，請記得複製並貼上這兩個指令檔。

## 擷取載入器指令碼 {#retrieve-the-loader-script}

1. 從樹狀結構中選取反向連結選件，然後按一下「 **反向連結選件動作** 」 **和「內嵌代碼」**。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 以滑鼠右鍵按一 **下頁首代碼** ，並將它插入網頁頁首。 然後，請對內文程式碼 **執行相同動作**。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 將指令碼貼到您的網頁上 {#pasting-the-scripts-onto-your-webpage}

將轉換指令碼貼入內文和標題的HTML。 接著，將載入器指令碼放入內文和標題的HTML中。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 連接轉換指令碼 {#connecting-the-conversion-script}

您將在此處編寫JavaScript函式，該函式使用您要觸發目標完成的任何頁面元素的特定HTML ID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此範例中，網頁上有一個ID為&quot;#myButtonId&quot;的按鈕。 按一下該按鈕後，會將該人員註冊為已完成目標。

太棒了！ 您的網站現在正透過Marketo擷取自訂的社交促銷目標。

>[!NOTE]
>
>**相關文章**
>
>* [指定反向連結選件的目標](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [建立反向連結選件](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [將Social部署在您的網站上](deploy-social-on-your-website.md)

