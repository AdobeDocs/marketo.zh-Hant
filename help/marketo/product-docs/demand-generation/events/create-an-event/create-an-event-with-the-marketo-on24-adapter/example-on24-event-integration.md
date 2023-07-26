---
unique-page-id: 10096679
description: ON24事件整合範例 — Marketo檔案 — 產品檔案
title: ON24事件整合範例
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 1%

---

# ON24事件整合範例 {#example-on-event-integration}

以下是ON24網路研討會的範例活動，包含行銷活動。 建立活動時，請務必在執行行銷活動之前先測試行銷活動。

## 在行銷活動中建立新事件 {#create-a-new-event-in-marketing-activities}

1. 選取 **新增** > **新計畫**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. 選取 **行銷活動資料夾** 活動將進行的位置。

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. 輸入 **名稱** 用於事件。

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. 選取 **事件** 作為 **計畫型別**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. 選取 **網路研討會** 作為 **頻道** 用於事件。

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. 按一下 **建立**。

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## 邀請（批次行銷活動）  {#invite-batch-campaign}

* **智慧清單**  — 定義您要邀請哪些人參加活動。
* **流程**

   * 傳送電子郵件 — 如果這是本機資產電子郵件，則有下列命名慣例： EventName.EmailName。 您也可以使用全域電子郵件。
   * 變更進度中的狀態 — 設定為網路研討會>已邀請。

* **排程**  — 設定傳送邀請的日期。

## 註冊/確認（觸發行銷活動） {#registration-confirmation-trigger-campaign}

* **智慧清單**

   * 觸發行銷活動依據 **填寫表單**. 一定要包含表單所在的登陸頁面，請使用 **新增限制**，尤其是表單用於多個登陸頁面時。

>[!CAUTION]
>
>您必須使用Marketo表單註冊事件人員，或非Marketo表單搭配適當的API整合，將註冊資料推送至Marketo。 這對於事件合作夥伴整合的成功至關重要。 **注意**：如果您在非Marketo登陸頁面上使用Marketo表單，則您的觸發程式會是 **填寫表單** 表單名稱。

![](assets/image2015-12-22-15-3a50-3a22.png)

* **流程**

   * **進度中的變更狀態**  — 設為「網路研討會>已註冊」。 **注意**：設定子行銷活動時，需要此流程步驟。 當個人的進度狀態變更為 **已註冊**，Marketo會將註冊資訊推送到ON24。

   * **傳送電子郵件**  — 確認電子郵件(設定為 **營運** 因此已註冊的取消訂閱者仍可接收)。

![](assets/image2015-12-22-15-3a52-3a9.png)

**注意**：如果人員因註冊錯誤而回訪，則不會收到電子郵件確認。

## 提醒（批次行銷活動） {#reminder-batch-campaign}

* **智慧清單**  — 篩選使用 **計畫成員** 並將狀態設為 **已註冊**.

* **流量**  — 傳送電子郵件（提醒電子郵件）。

**注意**：您可以使用類似的行銷活動來傳送 *不同* 後續追蹤電子郵件給已邀請但尚未註冊的人。

## 後續行銷活動（批次或觸發行銷活動） {#follow-up-campaign-batch-or-trigger-campaign}

* **智慧清單**  — 根據計畫狀態的變更觸發。

![](assets/image2015-12-22-15-3a57-3a25.png)

* **流量**  — 傳送電子郵件。 根據計畫狀態使用選項來傳送不同的電子郵件。

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
