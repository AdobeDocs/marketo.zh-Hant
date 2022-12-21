---
unique-page-id: 2359793
description: 在Social促銷活動中使用電子郵件 — Marketo檔案 — 產品檔案
title: 在社交促銷活動中使用電子郵件
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 在社交促銷活動中使用電子郵件 {#use-emails-in-social-promotions}

當您建立 [轉介優惠方案](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) 或 [抽獎活動](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以在人員註冊時傳送電子郵件，以及在人員獲得獎勵時再傳送。

>[!TIP]
>
>若要建立電子郵件，請參閱 [傳送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md).

在電子郵件中，使用下列代號：

* **註冊電子郵件**:使用 **`{{social.Share Url}}`** 傳送個人化分享連結給每個參與者。

* **履行電子郵件**:使用 **`{{social.Promo Code}}`** 傳送每個獲勝者 [促銷代碼](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>您必須先將電子郵件新增至社交應用程式，才能將其新增至 _操作_ 和 _核准_. 請參閱 [編輯電子郵件的設定](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. 前往 **行銷活動**.

   ![](assets/ma.png)

1. 選取應用程式，然後按一下 **編輯草稿**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交應用程式編輯器中，前往 **應用程式設定>選件詳細資料** (或 **抽獎活動詳細資訊**)。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 新增註冊電子郵件。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >當人員註冊時，系統會自動傳送確認電子郵件。

1. 新增履行電子郵件。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 在轉介優惠方案中，選擇自動還是手動傳送履行電子郵件。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>在抽獎活動中，當您 [選擇獲勝者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**定義**
>
>* **自動鎖定目標**:當每個參與者都達到目標時，會自動發送履行電子郵件。
>* **手動傳送**:當使用者開始達到目標時，請回到您的轉介選件以手動 [傳送履行電子郵件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>


>[!MORELIKETHIS]
>
>接下來，您可以 [選擇共用URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) 或者，在您的轉介選件中，您可以 [上傳促銷代碼](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) 你會派人出去的。
