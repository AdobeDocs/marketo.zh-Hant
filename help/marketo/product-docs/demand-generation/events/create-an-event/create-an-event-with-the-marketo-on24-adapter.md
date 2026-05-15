---
unique-page-id: 10096656
description: 瞭解如何使用Marketo ON24轉接器建立事件。 連線ON24網路研討會至Marketo，並同步註冊與出席情況。
title: 使用 Marketo ON24 Adapter 建立事件
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
TQID: https://experienceleague.adobe.com/LlMV9lfVxqvMh0E-6K3aStBiqOERGIKJOYSyJdaBvFw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 22%

---

# 使用 Marketo ON24 Adapter 建立事件 {#create-an-event-with-the-marketo-on-adapter}

您應熟悉在Marketo中建立事件的建置區塊和建議順序。 您也應該具備下列Marketo概念的實務知識：

* [Marketo計畫](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}以及事件，以及它們之間的差異
* [管道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [本地資產](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [子行銷活動](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}和[方案狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>如需Marketo API的詳細資訊，請參閱[Marketo API檔案](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

## 先決條件 {#prerequisites}

使用Marketo ON24整合需要下列專案：

* **訂閱ON24網路廣播** — 如果您沒有目前的訂閱，請直接連絡ON24。 **注意**：需要ON24託管版本。 不需要ON24事件管理。

* **ON24的管理員許可權** — 您需要此許可權才能使用此聯結器，並在ON24系統中建立來賓。
* **ON24連線認證** — 您必須在Marketo中輸入此資訊，才能啟用整合：使用者名稱、密碼、使用者端識別碼和使用者端金鑰。 如果您需要認證的相關協助，請連絡您的ON24客戶經理或ON24支援。
* **登錄檔單** — 使用Marketo表單或非Marketo表單以及適當的API，以確保註冊資料和註冊者資訊傳遞至Marketo。
* **註冊子行銷活動** — 您必須在Marketo事件中建立並正確設定註冊子行銷活動，事件合作夥伴整合才能運作。

## 處理流程 {#process-flow}

請依照下列步驟，使用Marketo On24轉接器建立事件：

1. [在 ON24 中建立您的網路研討會事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [設定事件設定並將 Marketo 與您的網路研討會同步](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [建立子系行銷活動和本地資產](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [測試您的 ON24 事件整合](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [ON24 事件整合範例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [了解網路研討會方案狀態](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [ON24 事件註冊更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
