---
unique-page-id: 10096656
description: 使用Marketo ON24適配器建立事件 — Marketo檔案 — 產品檔案
title: 使用Marketo ON24適配器建立事件
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 使用Marketo ON24適配器建立事件 {#create-an-event-with-the-marketo-on-adapter}

您應熟悉在Marketo中建立事件的建置區塊和建議順序。 您也應具備下列Marketo概念的實務知識：

* [Marketo計畫](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;}和事件，以及它們之間的差異
* [管道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target=&quot;_blank&quot;}
* [本機資產](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target=&quot;_blank&quot;}
* [子促銷活動](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}和 [方案狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>請參閱 [Marketo API檔案](https://developers.marketo.com/documentation/rest/){target=&quot;_blank&quot;}以取得Marketo API的詳細資訊。

## 必要條件 {#prerequisites}

使用Marketo ON24整合需要下列項目：

* **訂購ON24網路廣播**  — 如果您沒有當前訂閱，請直接與ON24聯繫。 **注意**:需要ON24托管版本。 ON24事件管理不是必需的。

* **ON24的管理員權限**  — 您需要此連接器，並在ON24系統中建立來賓。
* **ON24連接憑據**  — 您需要將此資訊輸入Marketo以啟用整合：用戶名、密碼、客戶端ID和客戶端密鑰。 如果貴機構需要有關憑證的幫助，請聯繫您的ON24客戶經理或ON24支援。
* **註冊表**  — 使用Marketo表單或非Marketo表單及適當的API，確保將註冊資料和註冊者資訊傳遞至Marketo。
* **註冊子項促銷活動**  — 您必須正確建立和設定Marketo事件中的註冊子促銷活動，事件合作夥伴整合才能正常運作。

## 流程 {#process-flow}

請依照下列步驟，使用Marketo On24適配器建立事件：

1. [在ON24中建立網路研討會活動](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target=&quot;_blank&quot;}
1. [設定事件設定並將Marketo與您的網路研討會同步](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}
1. [建立子促銷活動和本機資產](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target=&quot;_blank&quot;}
1. [測試您的ON24事件整合](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}
1. [ON24事件整合範例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
1. [了解網路研討會計畫狀態](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}
1. [ON24事件註冊更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;}
