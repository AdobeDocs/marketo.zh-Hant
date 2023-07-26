---
unique-page-id: 2359793
description: 在社交促銷活動中使用電子郵件 — Marketo檔案 — 產品檔案
title: 在社交促銷活動中使用電子郵件
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 在社交促銷活動中使用電子郵件 {#use-emails-in-social-promotions}

當您建立 [轉介優惠方案](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) 或 [抽獎](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以包含要在人員註冊時傳送的電子郵件，以及在人員贏得獎勵時再次傳送。

>[!TIP]
>
>若要建立電子郵件，請參閱 [傳送電子郵件爆炸訊息](/help/marketo/getting-started/quick-wins/send-an-email.md).

在電子郵件中，使用這些權杖：

* **註冊電子郵件**：使用 **`{{social.Share Url}}`** 傳送個人化共用連結給每位參與人員。

* **履行電子郵件**：使用 **`{{social.Promo Code}}`** 傳送每個獲勝者一個 [促銷代碼](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>您必須具備下列條件，才能將電子郵件新增至社交應用程式 _營運_ 和 _已核准_. 另請參閱 [編輯電子郵件的設定](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. 前往 **行銷活動**.

   ![](assets/ma.png)

1. 選取應用程式，然後按一下 **編輯草稿**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交應用程式編輯器中，前往 **應用程式設定>選件詳細資料** (或 **抽獎細節**)。

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
>在抽獎活動中，履行電子郵件一律會在您選擇後自動傳送 [選取獲勝者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**定義**
>
>* **目標上的自動**：當每位參與者達到目標時，會自動傳送履行電子郵件。
>* **手動傳送**：當人們開始達成目標後，請手動返回您的反向連結選件 [傳送履行電子郵件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>接下來，您可以 [選擇共用URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) 或者，在轉介優惠中，您可以 [上傳促銷代碼](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) 您將會送出。
