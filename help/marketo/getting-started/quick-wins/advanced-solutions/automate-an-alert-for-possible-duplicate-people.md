---
unique-page-id: 7513680
description: 自動提醒可能重複的人員——行銷人員檔案——產品檔案
title: 自動提醒可能重複的人員
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# 自動提醒可能重複的人員 {#automate-an-alert-for-possible-duplicate-people}

想在每次建立可能的重複人員時發出警報？ 以下是如何設定智慧型促銷活動來執行此動作。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

1. [建立新的智慧型促銷活動](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。 定義以下智慧清單：

   * 觸發器： **建立人員**
   * 篩選：**重複欄位。 **欄位名稱 **為****完整名稱**。

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >發揮創意。 嘗試不同的欄位，以取得更佳的篩選結果。

1. 在流程步驟中，選擇「發送 [警報流程](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 」操作。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >使用 [傳送警報資訊Token](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) ，在CRM中包含人員的連結。

   >[!CAUTION]
   >
   >如果您匯入大型清單，可能會同時收到許多警報！
   >
   >
   >另外，兩個同名的人並不自動表示他們是同一個人。

1. 在「排程」標籤中啟 **用促銷** 活動。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

就這樣！ 每當在Marketo中建立現有全名的新人時，就會觸發此智慧型促銷活動。

>[!MORELIKETHIS]
>
>* [查找並合併重複人員](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

