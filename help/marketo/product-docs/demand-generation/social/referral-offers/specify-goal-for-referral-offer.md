---
unique-page-id: 2359791
description: 指定轉介優惠的目標 — Marketo檔案 — 產品檔案
title: 指定轉介優惠的目標
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# 指定轉介優惠的目標 {#specify-goal-for-referral-offer}

當您[建立轉介優惠方案](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)時，您必須定義履行目標。 目標可由網頁上的個人活動定義，例如頁面瀏覽或註冊。 您甚至可以使用[自訂JavaScript事件](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)。

或者，您可以使用Marketo中的智慧清單觸發器，等待任何里程碑，例如為轉介的人員建立的機會。

目標範例：

* 10次轉介的造訪
* 5個引用的註冊
* 已建立1個轉介的機會
* 2次引用的電子商務購買
* 5位轉介的網路研討會與會者

1. 移至&#x200B;**行銷活動**。

   ![](assets/ma.png)

1. 選取轉介優惠方案，然後按一下&#x200B;**編輯草稿**。

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在轉介選件編輯器中，移至&#x200B;**應用程式設定** > **選件詳細資料**。

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 在「**設定**」下，從「**履行目標**」下拉式清單中選擇事件型別。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您打算使用&#x200B;**將評分給予反向連結**&#x200B;流程步驟，您必須在此選取&#x200B;**智慧清單觸發程式**&#x200B;作為履行目標型別。

* 轉介的造訪：優惠方案參與者可獲得朋友每次造訪您優惠方案所在頁面時的點數。
* 轉介的註冊：優惠方案參與者可獲得每個已註冊優惠方案的朋友的評分。
* 智慧清單觸發程式：優惠方案參與者可獲得[智慧行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)中符合[智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)觸發程式條件的每個朋友的評分。 例如，您可使用觸發器，當被轉介的潛在客戶註冊網路研討會時引發。

* 自訂JavaScript事件：為頁面上觸發已定義JavaScript事件的每個朋友，提供優惠方案給參與者以評分。 檢視自訂事件的[轉換指令碼](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>智慧型行銷活動中提供新的篩選器和觸發器，可用於監控社交活動。 請參閱[使用社交活動的觸發器和篩選器](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!MORELIKETHIS]
>
>接著，您可以[選取註冊和履行電子郵件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)，以從您的推薦優惠傳送。
