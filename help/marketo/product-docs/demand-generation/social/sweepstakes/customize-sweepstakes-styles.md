---
unique-page-id: 2359807
description: 自訂抽獎樣式 — Marketo檔案 — 產品檔案
title: 自訂抽獎樣式
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# 自訂抽獎樣式 {#customize-sweepstakes-styles}

當您[建立抽獎活動](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)時，您可以自訂它在您的登陸頁面上的外觀。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 無法再建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

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
