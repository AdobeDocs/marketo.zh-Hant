---
unique-page-id: 1147091
description: 瞭解計畫成員資格 — Marketo檔案 — 產品檔案
title: 瞭解計畫會員資格
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: eb6d834c1f430beebf0666d7694203a268be93f2
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 瞭解計畫會員資格 {#understanding-program-membership}

>[!NOTE]
>
>Marketo現在正對所有訂閱的語言進行標準化，因此您可能會在訂閱中看到銷售機會/銷售機會，並在我們的檔案中看到相關人員。 這些詞語的意思相同；它不會影響文章指示。 此外也有其他變更。 [深入瞭解](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md){target="_blank"}。

>[!NOTE]
>
>**定義：**&#x200B;成員是在方案中擁有狀態的人員。

## 人們如何成為計畫的成員 {#how-people-become-members-of-a-program}

1. 某人填寫程式中登入頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}上的[表單。

   1. 人員會自動擁有進度中的第一個狀態。

1. 您從CSV檔案[將成員匯入程式](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"}。

   1. 人員會自動擁有進度中的第一個狀態。

1. 您使用[變更程式狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}流程步驟。
1. 人員註冊或出席與活動程式](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md){target="_blank"}同步的[網路研討會。
1. 已使用Marketo iPad簽入應用程式](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md){target="_blank"}建立人員[。
1. 已將人員新增至SFDC行銷活動，此行銷活動已[同步至方案](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}。

>[!NOTE]
>
>若是電子郵件方案，則只有在傳送電子郵件後，才會將個人新增至會籍。

## 計畫狀態 {#program-statuses}

計畫狀態是人們在計畫中執行的步驟（例如，已邀請、已回覆、已參加、無節目）。 這些步驟由[管道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}定義。

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>人員無法回到先前的計畫狀態。 狀態進度僅為單向。

## 成功狀態 {#success-statuses}

方案的目的是建立與人員或潛在客戶的有意義的互動。 當個人達到達到達到該目標的狀態時會標籤成功。

>[!NOTE]
>
>就網路研討會而言，如果註冊實際上並未觀看網路研討會，則其意義不大。 在這種情況下，出席是成功的。

## 贏取方案 {#acquisition-program}

當新名稱進入系統作為方案成員時，Marketo會自動將該方案設為「贏取」。 這會建立[首次接觸歸因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md){target="_blank"}的評分。

>[!MORELIKETHIS]
>
>* [在程式中使用標籤](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/use-tags-in-a-program.md){target="_blank"}
>* [建立方案效能報告](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md){target="_blank"}
