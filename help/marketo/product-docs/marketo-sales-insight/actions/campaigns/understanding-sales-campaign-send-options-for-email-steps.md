---
description: 瞭解電子郵件步驟的Sales Campaign傳送選項 — Marketo檔案 — 產品檔案
title: 瞭解電子郵件步驟的Sales Campaign傳送選項
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 瞭解電子郵件步驟的Sales Campaign傳送選項 {#understanding-sales-campaign-send-options-for-email-steps}

當您建立促銷活動時，您有幾個選項可讓您決定如何在[!DNL Sales Insight Actions]中建立電子郵件步驟。 此外，視您的電子郵件在促銷活動中的位置而定，您的選項也會有所不同。

## 第一步傳送選項 {#first-step-send-options}

如果這是您促銷活動的第一個步驟和第一天，您將有下列選項：

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### 我將選擇何時傳送此電子郵件 {#first-step-i-will-choose}

* 此選項可讓您在新增人員以啟動促銷活動時，為促銷活動中的第一封電子郵件選擇「傳送時間」時間。

### 在下列時間傳送此電子郵件 {#first-step-following-time}

* 當您透過新增人員來開始您的促銷活動時，我們將排程此時段的電子郵件。
* 您一律可以選擇在展開促銷活動時選擇新的「傳送時間」。

### 建立任務；我自己會傳送這封電子郵件 {#first-step-create-a-task}

* 此選項將建立您可方便傳送的電子郵件工作（並同步至[!DNL Salesforce]）。
* 當您完成此選取後，當您開始促銷活動時，我們會在指揮中心和即時摘要為您佇列這些工作。 接著，您就可以個人化，並在電子郵件傳送前傳送（或排程）每封電子郵件。

   * 如果您在Web應用程式中開啟此工作，則會開啟撰寫視窗，其中包含連絡人的電子郵件地址、電子郵件的主旨行以及您選擇的範本。
   * 如果您在Gmail或[!DNL Outlook]中開啟此工作，則會開啟原生撰寫視窗，並動態填入連絡人的電子郵件地址、電子郵件的主旨行以及您選擇的範本。

## 後續步驟傳送選項 {#subsequent-step-send-options}

對於銷售行銷活動中的任何後續天數/步驟，您有以下選項：

### 與此銷售行銷活動中的上一封電子郵件同時傳送此電子郵件 {#subsequent-send-at-same-time}

* 此選項會在電子郵件直接發出的同時傳送電子郵件。
* 它仍會在相關聯的當天傳送。

>[!IMPORTANT]
>
>同日傳送的電子郵件不支援在上一個電子郵件同時傳送電子郵件。 相反地，電子郵件會在前一天傳送的電子郵件時發出。 如果針對行銷活動第一天的電子郵件選取此選項（不建議），則該電子郵件將在行銷活動開始時立即寄出。

### 在下列時間傳送此電子郵件 {#subsequent-send-at-following-time}

* 當您透過新增人員來開始您的促銷活動時，我們將排程此時段的電子郵件。
* 您一律可以選擇在展開促銷活動時選擇新的「傳送時間」。

### 建立任務；我自己會傳送這封電子郵件 {#subsequent-create-a-task}

* 此選項將建立您可方便傳送的電子郵件工作（並同步至[!DNL Salesforce]）。
* 完成此選取後，當您開始銷售行銷活動時，[!DNL Sales Insight Actions]會在指揮中心和即時摘要中為您佇列這些任務。 接著，您就可以個人化，並在電子郵件傳送前傳送（或排程）每封電子郵件。

   * 如果您在Web應用程式中開啟此工作，則會開啟撰寫視窗，其中包含連絡人的電子郵件地址、電子郵件的主旨行以及您選擇的範本。
   * 如果您在Gmail或[!DNL Outlook]中開啟此工作，則會開啟原生撰寫視窗，並動態填入連絡人的電子郵件地址、電子郵件的主旨行以及您選擇的範本。

### 建立此電子郵件，作為此行銷活動中前一封電子郵件的後續追蹤 {#subsequent-create-this-email}

* 如果您想要將促銷活動中的前一封電子郵件附加至促銷活動傳送的下一封電子郵件，請啟用此核取方塊。
* 對於電子郵件的附加副本，您促銷活動中的電子郵件範本將一律寄出。 使用者在傳送之前所做的任何編輯都不會包含在傳送中。

>[!NOTE]
>
>建立電子郵件作為後續的選項，僅在電子郵件步驟中可用，當上一個步驟也是電子郵件時。 如果前一步為「呼叫」、「InMail」或「自訂」，則不會顯示建立後續追蹤的選項。

>[!MORELIKETHIS]
>
>[建立促銷活動](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>&#x200B;>[銷售行銷活動步驟型別和提醒任務](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>&#x200B;>[銷售促銷活動設定](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}

