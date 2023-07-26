---
unique-page-id: 1147091
description: 瞭解計畫成員資格 — Marketo檔案 — 產品檔案
title: 瞭解計畫會員資格
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 瞭解計畫會員資格 {#understanding-program-membership}

>[!NOTE]
>
>Marketo現在正對所有訂閱的語言進行標準化，因此您可能會在訂閱中看到銷售機會/銷售機會，並在我們的檔案中看到相關人員。 這些詞語的意思相同；它不會影響文章指示。 此外也有其他變更。 [深入了解](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**定義：** 成員是在方案中擁有狀態的人員。

## 人們如何成為計畫的成員 {#how-people-become-members-of-a-program}

1. 某人填寫 [登陸頁面上的表單](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) 在程式中。

   1. 人員會自動擁有進度中的第一個狀態。

1. 您 [將成員匯入程式](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) 從CSV檔案。

   1. 人員會自動擁有進度中的第一個狀態。

1. 您使用 [變更方案狀態](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) 流程步驟。
1. 個人註冊或出席 [與活動方案同步的網路研討會](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md).
1. 個人是 [使用Marketo iPad簽入應用程式建立](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. 新增人員至SFDC促銷活動，也就是 [已同步至程式](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>若是電子郵件方案，則只有在傳送電子郵件後，才會將個人新增至會籍。

## 計畫狀態 {#program-statuses}

計畫狀態是人們在計畫中執行的步驟（例如，已邀請、已回覆、已參加、無節目）。 這些步驟由以下定義 [頻道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>人員無法回到先前的計畫狀態。 狀態進度僅為單向。

## 成功狀態 {#success-statuses}

方案的目的是建立與人員或潛在客戶的有意義的互動。 當個人達到達到達到該目標的狀態時會標籤成功。

>[!NOTE]
>
>就網路研討會而言，如果註冊實際上並未觀看網路研討會，則其意義不大。 在這種情況下，出席是成功的。

## 贏取方案  {#acquisition-program}

當新名稱進入系統作為方案成員時，Marketo會自動將該方案設為「贏取」。 這將建立以下專案的信用 [首次接觸歸因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [在程式中使用標籤](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [建立方案效能報表](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)
