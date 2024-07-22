---
unique-page-id: 2359807
description: 自訂抽獎樣式 — Marketo檔案 — 產品檔案
title: 自訂抽獎樣式
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# 自訂抽獎樣式 {#customize-sweepstakes-styles}

當您[建立抽獎活動](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)時，您可以自訂它在您的登陸頁面上的外觀。

>[!AVAILABILITY]
>
>並非所有Marketo Engage使用者都已購買此功能。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

1. 移至&#x200B;**行銷活動**。

![](assets/login-marketing-activities-1.png)

1. 選取抽獎活動，然後按一下&#x200B;**編輯草稿**。

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 在Sweepstakes編輯器中，移至&#x200B;**應用程式設定** > **外觀**。

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 編輯您的註冊按鈕和進度連結的文字。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. 針對您要自訂的每個元素，輸入自訂CSS屬性。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   **輸入按鈕**的CSS範例：
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   **Enter按鈕**的影像範例：
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >如果您使用上面有文字的影像，請記得從上方文字下方的&#x200B;**輸入按鈕**&#x200B;欄位中移除文字。

1. 每次進行變更時，結果都會顯示在「檢視和編輯」預覽中。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >在多種不同的瀏覽器中測試您的按鈕，包括舊版。

   >[!MORELIKETHIS]
   >
   >下一步是新增[註冊與履行電子郵件至您的抽獎活動](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md)。
