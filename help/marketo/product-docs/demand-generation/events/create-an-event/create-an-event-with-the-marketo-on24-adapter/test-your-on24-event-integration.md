---
unique-page-id: 10096677
description: 測試您的ON24事件整合——行銷檔案——產品檔案
title: 測試您的ON24事件整合
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# 測試您的ON24事件整合{#test-your-on-event-integration}

請務必徹底測試您的事件整合。

## 執行第一個促銷活動前建議的測試順序{#recommended-test-sequence-before-running-your-first-campaign}

1. 填寫活動的註冊表單，並使用有效的電子郵件地址進行測試。
1. 在Marketo事件的「會籍」格線中，確認測試名稱顯示為&#x200B;**已註冊**&#x200B;狀態。
1. 確認測試名稱在ON24中也顯示為&#x200B;**Registered**。
1. 確認您用來註冊測試名稱的有效電子郵件地址收到確認電子郵件給「事件」，且電子郵件中已解決唯一URL。

   >[!NOTE]
   >
   >您必須在確認電子郵件中使用`{{member.webinar url}}`代號，才能在每位註冊者的電子郵件中顯示唯一URL。

## 事件{#after-the-event}之後

以下是事件發生後資料的更新方式：

* Marketo每晚從ON24擷取參與者資料。
* 當參與者資料在Marketo和ON24之間同步後，Marketo會將會籍狀態更新為「已出席」、「已參加隨選」或「無顯示」。 在事件的&#x200B;**摘要**&#x200B;標籤中，事件狀態更新為&#x200B;**事件完成**。

>[!MORELIKETHIS]
>
>* [ON24事件整合範例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [瞭解Marketo ON24適配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

