---
unique-page-id: 2359807
description: 自訂抽獎活動樣式 — Marketo檔案 — 產品檔案
title: 自訂抽獎活動樣式
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# 自訂抽獎活動樣式 {#customize-sweepstakes-styles}

當您 [建立抽獎活動](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以自訂其在登陸頁面上的外觀。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的銷售代表。

1. 前往 **行銷活動**.

![](assets/login-marketing-activities-1.png)

1. 選取抽獎活動，然後按一下 **編輯草稿**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 在抽獎活動編輯器中，前往 **應用程式設定** > **外觀**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 編輯註冊按鈕和進度連結的文本。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. 針對您要自訂的每個元素，輸入您的自訂CSS屬性。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   範例CSS **輸入按鈕**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   範例影像 **輸入按鈕**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >如果您使用的影像上有文字，請記得從 **輸入按鈕** 欄位。

1. 每次更改時，結果都顯示在「視圖和編輯」(View &amp; Edit)預覽中。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >在數個不同的瀏覽器中測試您的按鈕，包括舊版。

   >[!MORELIKETHIS]
   >
   >下一步是新增 [註冊和履行電子郵件給您的抽獎活動](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
