---
unique-page-id: 1147091
description: 瞭解方案會員-Marketo文檔——產品文檔
title: 瞭解方案會籍
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 瞭解方案會員{#understanding-program-membership}

>[!NOTE]
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)。

>[!NOTE]
>
>**定義：** 成員是具有方案狀態的人員。

## 人們如何成為程式成員{#how-people-become-members-of-a-program}

1. 人員填寫程式中登陸頁面上的[表格。](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

   1. 人員將自動擁有晉升中的第一個狀態。

1. 您[從CSV檔案將成員導入程式](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md)。

   1. 人員將自動擁有晉升中的第一個狀態。

1. 您使用[change program status](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)流步驟。
1. 有人會註冊或參加與事件程式](/help/marketo/product-docs/demand-generation/events/understanding-events/launchpoint-event-partners.md)同步的[網路研討會。
1. 使用MarketoiPad登入應用程式](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md)建立人員。[
1. 將人員添加到SFDC促銷活動，該促銷活動與程式](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)同步。[

>[!NOTE]
>
>對於電子郵件方案，只有在傳送電子郵件時，才會將人員新增至會籍。

## 程式狀態{#program-statuses}

方案狀態是人們在方案中執行的步驟（例如，已邀請、RSVPd、已參加、無顯示）。 這些步驟由[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)定義。

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>人員無法向後移至先前的程式狀態。 狀態晉升只是一種方式。

## 成功狀態{#success-statuses}

程式的目的，是與人或潛在客戶建立有意義的互動。 當某人達到達到該目標的狀態時，就會標籤成功。

>[!NOTE]
>
>在網路研討會中，如果註冊並不是真正觀看網路研討會的有意義互動。 在這種情況下，主治是成功的。

## 收購計畫{#acquisition-program}

當新名稱以方案會員身分進入系統時，Marketo會自動將該方案設為「贏取」。 這可建立[首次接觸歸因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)的評分。

>[!MORELIKETHIS]
>
>* [在程式中使用標籤](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [建立方案績效報告](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

