---
unique-page-id: 2359791
description: 指定轉介優惠的目標 — Marketo檔案 — 產品檔案
title: 指定轉介優惠的目標
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 指定轉介優惠的目標 {#specify-goal-for-referral-offer}

當您 [建立轉介優惠方案](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)，您必須定義履行目標。 目標可由網頁上的個人活動定義，例如頁面瀏覽或註冊。 您甚至可以使用 [自訂JavaScript事件](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

或者，您可以使用Marketo中的智慧清單觸發程式來等待任何里程碑，例如為被引薦人員建立的商機。

目標範例：

* 10次轉介的造訪
* 5個引用的註冊
* 已建立1個轉介的機會
* 2個引用的電子商務購買
* 5位被推薦的網路研討會與會者

1. 前往 **行銷活動**.

   ![](assets/ma.png)

1. 選取反向連結選件，然後按一下 **編輯草稿**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在反向連結選件編輯器中，前往 **應用程式設定** > **優惠方案詳細資料**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 下 **設定**，從中選擇事件型別 **履行目標** 下拉式清單。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您打算使用 **將評分給予反向連結** 流程步驟，您必須選取 **智慧清單觸發程式** 作為履行目標型別。

* 反向造訪：優惠方案參與者可獲得朋友每次造訪託管優惠方案之頁面的點數。
* 轉介註冊：優惠參與者可獲得每個已註冊優惠之朋友的評分。
* 智慧清單觸發程式：優惠方案參與者可獲得每個符合條件的朋友的評分。 [智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) 在中觸發 [智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). 例如，當被轉介的潛在客戶註冊網路研討會時，您可以使用觸發程式。

* 自訂JavaScript事件：優惠方案參與者可獲得頁面上觸發已定義JavaScript事件的朋友的評分。 另請參閱 [自訂事件的轉換指令碼](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>智慧型行銷活動中有新的篩選器和觸發器可用來監視社交活動。 另請參閱 [對社交活動使用觸發器和篩選器](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>接下來，您可以 [選取註冊與履行電子郵件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) 以從您的轉介優惠傳送。
