---
unique-page-id: 2359807
description: 自訂抽獎活動樣式——行銷檔案——產品檔案
title: 自訂抽獎活動樣式
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# 自訂抽獎活動樣式{#customize-sweepstakes-styles}

當您[建立抽獎活動](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)時，您可以自訂其在登陸頁面上的外觀。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請洽詢您的銷售代表。

1. 前往&#x200B;**行銷活動**。

![](assets/login-marketing-activities-1.png)

1. 選取抽獎活動，然後按一下「編輯草稿」。****

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 在抽獎活動編輯器中，前往「應用程式設定」**>>「外觀」**>。****

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 編輯註冊按鈕和進度連結的文字。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. 針對您要自訂的每個元素，輸入您的自訂CSS屬性。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   **Enter Button**的CSS範例：
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   **輸入按鈕**的範例影像：
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >如果您使用的影像上有文字，請記得從上方「文字」下方的「輸入按鈕&#x200B;**」欄位中移除文字。**

1. 每次進行變更時，結果會顯示在「檢視與編輯」預覽中。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >在多種不同的瀏覽器（包括舊版）中測試您的按鈕。

   >[!MORELIKETHIS]
   >
   >下一步是將[註冊和履約電子郵件新增至您的抽獎活動](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md)。
