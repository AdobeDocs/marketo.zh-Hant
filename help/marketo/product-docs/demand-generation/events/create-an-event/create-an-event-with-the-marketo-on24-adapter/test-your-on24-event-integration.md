---
unique-page-id: 10096677
description: 測試您的ON24事件整合 — Marketo檔案 — 產品檔案
title: 測試您的ON24事件整合
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# 測試您的ON24事件整合 {#test-your-on-event-integration}

請務必徹底測試您的事件整合。

## 執行第一個行銷活動前的建議測試順序 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填寫事件的登錄檔單，並使用有效的電子郵件地址進行測試。
1. 確認顯示的測試名稱包含 **已註冊** Marketo事件之「成員資格」格線中的狀態。
1. 確認測試名稱也顯示為 **已註冊** 於ON24。
1. 確認您用來註冊測試名稱的有效電子郵件地址已收到一封確認電子郵件給事件，且唯一URL已在電子郵件中解析。

   >[!NOTE]
   >
   >您必須使用 `{{member.webinar url}}` 記號，以便在每位註冊者的電子郵件中顯示唯一的URL。

## 在事件之後 {#after-the-event}

以下是事件發生後如何更新資料：

* Marketo每晚都會從ON24擷取出席者資料。
* 在與會者資料在Marketo和ON24之間同步後，Marketo會將會籍狀態更新為已參加、已出席隨選或未顯示。 在事件的 **摘要** 索引標籤中，事件狀態會更新為 **事件完成**.

>[!MORELIKETHIS]
>
>* [ON24事件整合範例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
