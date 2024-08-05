---
unique-page-id: 2359793
description: 在社交促銷活動中使用電子郵件 — Marketo檔案 — 產品檔案
title: 在社交促銷活動中使用電子郵件
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# 在社交促銷活動中使用電子郵件 {#use-emails-in-social-promotions}

當您建立[轉介優惠方案](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)或[抽獎](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)時，您可以加入電子郵件以在人員註冊時傳送，並在人員贏得獎勵時再次傳送。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 您將無法建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!TIP]
>
>若要建立電子郵件，請參閱[傳送電子郵件爆炸訊息](/help/marketo/getting-started/quick-wins/send-an-email.md)。

在電子郵件中，使用這些權杖：

* **註冊電子郵件**：使用&#x200B;**`{{social.Share Url}}`**&#x200B;傳送個人化共用連結給每位參與者。

* **履行電子郵件**：使用&#x200B;**`{{social.Promo Code}}`**&#x200B;傳送促銷代碼](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)給每位獲勝者。[

>[!PREREQUISITES]
>
>您必須是&#x200B;_營運_&#x200B;和&#x200B;_已核准_，才能將電子郵件新增至社交應用程式。 請參閱[編輯電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)的設定。

1. 移至&#x200B;**行銷活動**。

   ![](assets/ma.png)

1. 選取應用程式，然後按一下&#x200B;**編輯草稿**。

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交應用程式編輯器中，前往&#x200B;**應用程式設定>選件詳細資料** （或&#x200B;**抽獎詳細資料**）。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 新增註冊電子郵件。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >當有人註冊時，會自動傳送確認電子郵件。

1. 新增履行電子郵件。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 在推薦優惠中，選擇履行電子郵件是自動還是手動傳送。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>在抽獎活動中，當您[選取獲勝者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)時，永遠會自動傳送履行電子郵件。

>[!NOTE]
>
>**定義**
>
>* 目標&#x200B;**上的**&#x200B;自動：當每位參與者達到目標時，會自動傳送履行電子郵件。
>* **手動傳送**：一旦人們開始達成目標，請返回您的轉介優惠以手動[傳送履行電子郵件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)。
>

>[!MORELIKETHIS]
>
>接著，您可以[選擇共用URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)，或在您的轉介選件中，您可以[上傳要傳送的促銷代碼](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)。
