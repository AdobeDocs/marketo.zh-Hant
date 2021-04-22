---
unique-page-id: 7513680
description: 自動提醒可能重複的人員-Marketo文檔——產品文檔
title: 自動提醒可能重複的人員
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 自動發出可能重複的人員警報{#automate-an-alert-for-possible-duplicate-people}

想在每次建立可能的重複人員時發出警報？ 以下是如何設定智慧型促銷活動來執行此動作。

1. [建立新的智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。定義以下智慧清單：

* 觸發器：**已建立人員**
* 篩選：**重複欄位。** 欄位名稱 **為完整名稱**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >發揮創意。 嘗試不同的欄位，以取得更佳的篩選結果。

1. 在流步驟中，選擇[發送警報](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)流操作。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >使用[傳送警報資訊Token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md)在CRM中包含該人員的連結。

   >[!CAUTION]
   >
   >如果您匯入大型清單，可能會同時收到許多警報！
   >
   >另外，兩個同名的人並不自動表示他們是同一個人。

1. 在&#x200B;**「排程**」標籤中啟用促銷活動。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

就這樣！ 每次在Marketo建立現有全名新人員時，都會觸發此智慧型促銷活動。

>[!MORELIKETHIS]
>
>[查找並合併重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
