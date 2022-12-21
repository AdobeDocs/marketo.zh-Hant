---
unique-page-id: 10096677
description: 測試您的ON24事件整合 — Marketo檔案 — 產品檔案
title: 測試您的ON24事件整合
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# 測試您的ON24事件整合 {#test-your-on-event-integration}

請務必徹底測試事件整合。

## 執行第一個促銷活動之前的建議測試順序 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填寫事件的註冊表，並使用有效的電子郵件地址進行測試。
1. 確認測試名稱顯示為 **已註冊** 狀態(在Marketo事件的「成員資格」格線中)。
1. 確認測試名稱也顯示為 **已註冊** 在ON24。
1. 確認您用來註冊測試名稱的有效電子郵件地址收到一封確認電子郵件給事件，且電子郵件中已解析唯一URL。

   >[!NOTE]
   >
   >您必須使用 `{{member.webinar url}}` 確認電子郵件中的代號，以便在每個註冊者的電子郵件中顯示唯一URL。

## 事件之後 {#after-the-event}

以下是發生事件後資料的更新方式：

* Marketo每晚從ON24中檢索與會者資料。
* 在Marketo和ON24之間同步與會者資料後，Marketo會將會員狀態更新為「已出席」、「隨選已出席」或「無節目」。 在活動中 **摘要** 標籤中，事件狀態會更新為 **事件完成**.

>[!MORELIKETHIS]
>
>* [ON24事件整合範例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
>* [了解Marketo ON24適配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}

