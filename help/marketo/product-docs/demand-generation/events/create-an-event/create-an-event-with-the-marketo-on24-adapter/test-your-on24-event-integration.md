---
unique-page-id: 10096677
description: 測試您的ON24事件整合——行銷檔案——產品檔案
title: 測試您的ON24事件整合
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# 測試您的ON24事件整合 {#test-your-on-event-integration}

請務必徹底測試您的事件整合。

## 執行第一個促銷活動前建議的測試順序 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填寫活動的註冊表單，並使用有效的電子郵件地址進行測試。
1. 在Marketo事件的「會籍」格 **線中** ，確認測試名稱顯示為已註冊狀態。
1. 確認測試名稱在ON24中也 **顯示為** 「已註冊」。
1. 確認您用來註冊測試名稱的有效電子郵件地址收到確認電子郵件給「事件」，且電子郵件中已解決唯一URL。

   >[!NOTE]
   >
   >您必須在確認 `{{member.webinar url}}` 電子郵件中使用代號，才能在每位註冊者的電子郵件中顯示唯一URL。

## 事件後 {#after-the-event}

以下是事件發生後資料的更新方式：

* Marketo每晚從ON24擷取參與者資料。
* 當參與者資料在Marketo和ON24之間同步後，Marketo會將會籍狀態更新為「已出席」、「已參加隨選」或「無顯示」。 在事件的「摘 **要** 」標籤中，事件狀態會更新為「事 **件完成」**。

>[!NOTE]
>
>**相關文章**
>
>* [ON24事件整合範例](example-on24-event-integration.md)
>* [瞭解Marketo ON24適配器事件](understanding-marketo-on24-adapter-events.md)

>



