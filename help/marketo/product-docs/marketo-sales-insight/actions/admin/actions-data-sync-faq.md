---
description: Actions資料同步常見問題集 — Marketo檔案 — 產品檔案
title: 動作資料同步常見問題集
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: fbeb28b1b89fb329a4b45fb01dbad7df939ddc0c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# 動作資料同步常見問題集 {#actions-data-sync-faq}

Sales Insight Actions的資料統一欄位同步使系統能夠將人員資訊從您的Marketo Engage資料庫提取到您的Sales Insight Actions資料庫中。

這可在Sales Insight Actions Web應用程式中提供最新的人員資料，並允許系統為Marketo中的對應人員記錄和Salesforce中的銷售機會/聯繫人/帳戶/機會記錄收集唯一ID，以便記錄資料可被正確引用。

您可以從Marketo Engage的「管理員」區段的「銷售分析動作設定」標籤啟用此同步。 如需詳細資訊，請查看 [啟動資料同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

上圖顯示人員活動和任務資料在系統之間如何同步。 請注意以下幾點：

* 人員記錄會從Marketo Engage同步至「銷售分析動作」，使Marketo Engage成為「銷售分析動作」人員資料的真實來源
* Marketo Engage和銷售分析操作 [有機制](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) 用於收集和同步取消訂閱狀態到Salesforce
* 取消訂閱狀態不會從「銷售活動」同步到「Marketo Engage」，但可以配置「銷售分析活動」以在允許銷售者發送電子郵件之前檢查人員的「Marketo取消訂閱」狀態 [Marketo取消訂閱檢查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

以下是與資料統一同步如何運作相關的一些常見問題。

## 哪些銷售機會/聯繫人已同步至Sales Insight Actions? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

將將分配給銷售責任人的銷售機會和聯繫人下一步同步到銷售活動。

您可以查看存在的標準責任人欄位，查看銷售線索/聯繫人在Salesforce中是否具有銷售責任人。

銷售擁有者不必是Marketo同步使用者或任何特定的Salesforce或銷售使用者。 我們只需要在Salesforce中列出的銷售線索責任人和聯繫人責任人欄位上列出一個用戶，這樣我們就可以將其標識為銷售線索，並將其同步到Sales Insight Actions中。 我們與同步的欄位的任何更新也會在Sales Insight Actions中偵測並更新。

## 顯示在Sales Insight Smart Grid中的活動資料從何處獲得來源？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

活動資料（例如電子郵件、呼叫、有趣的時刻和網頁）均源自於Marketo Engage的資料庫。 Sales Insight Smart Grid會向Marketo Engage實例提出請求，以在每次銷售用戶載入Sales Insight面板時檢索此實例。

![](assets/actions-data-sync-faq-4.png)

為確保所有活動資料均可源自Marketo Engage，「銷售分析活動」會將所有活動資料同步至Marketo Engage。

## 與人員記錄相關的哪些欄位從Marketo Engage同步到Sales Insight Actions? {#what-fields-sync}

有11個欄位會從Marketo Engage同步至Sales Insight Actions:

* 名字
* 姓氏
* Salesforce聯繫人ID
* Salesforce銷售線索ID
* Salesforce帳戶ID
* Salesforce機會ID
* Marketo ID
* 公司
* 標題
* 電子郵件
* 電話號碼
* Linkedin URL
* 來源

## 在Marketo Engage和Sales Insight Actions之間同步的欄位是否可配置？ {#are-the-fields-that-sync-configurable}

無法設定同步到Sales Insight Actions的Marketo Engage欄位，也無法映射欄位。 從Marketo同步會自動將標準Marketo欄位對應至您「銷售動作」例項中的標準欄位。

## Sales Insight Actions為何有其自己的資料庫？ {#why-does-actions-have-its-own-database}

Sales Insight Actions擁有自己的Web應用程式，其中包含專用的人員和活動資料庫，以提供為銷售團隊構建和設計的優化工作區。 這使銷售經理和銷售商能夠有空間構建和管理其參與策略，而不授予對主要Marketo Engage工作區的訪問權或權限，該工作區是針對市場營銷操作專家而優化的。

## 如何處理重複項？ {#how-are-duplicates-handled}

您的銷售活動資料庫將是存在於Marketo Engage資料庫中的合格人員（銷售負責人/聯繫人）的副本。 這表示，如果在Marketo中建立了兩個具有相同電子郵件地址的記錄，則在Sales Actions中將會建立重複的記錄。

## 完成初始同步需要多久時間？ {#how-long-initial-sync}

將所有銷售線索資料同步到新的「銷售分析活動」實例的初始過程通常每1-2分鐘處理1,000人。 這只是一個估計值，可能會有所不同。

一旦初始同步完成，且您的所有銷售線索都已填充到您的Sales Insight Actions Web應用程式實例中後，每當有一個更新被同步的受支援欄位時，就會運行增量同步。

## Sales Insight Actions使用者是否可編輯Actions網頁應用程式中的人員資料？ {#can-actions-users-edit-people-data}

否，動作網頁應用程式的使用者和管理員無法在動作中建立及編輯人員記錄。 建立和編輯人員必須在Salesforce或Marketo Engage中完成。 Sales Insight Actions會持續同步新資料，將Marketo當作人員資料的真實來源，因此，如果在Marketo中從Marketo的工作流程更新或建立人員，或從Salesforce同步，這些更新將會傳遞至Sales Insight Actions網頁應用程式資料庫。

## 銷售活動是否登錄到Marketo? {#do-sales-activities-log-to-marketo}

是的，銷售參與活動將以原生活動登入Marketo。 這些活動還包括原生篩選器，可搭配限制使用，以根據銷售活動屬性來定位銷售機會。

![](assets/actions-data-sync-faq-5.png)

以下是登入Marketo的活動清單：

* 發送銷售電子郵件
* 開啟銷售電子郵件
* 按一下銷售電子郵件
* 已回覆銷售電子郵件
* 已退回銷售電子郵件
* 已接收銷售呼叫
* 添加到銷售活動
* 從Sales Campaign中移除

## 銷售活動是否登錄到Salesforce? {#do-sales-activities-log-to-salesforce}

是的，銷售參與活動將作為本機任務登錄到Salesforce。 然後，這些任務便可在Salesforce報表中使用，以支援追蹤銷售活動的團隊控制面板。

「銷售分析動作」可讓管理員設定要記錄到Salesforce的銷售活動。 這些活動包括電子郵件、呼叫和未結提醒任務。

![](assets/actions-data-sync-faq-6.png)

上圖顯示了哪些資訊記錄到Salesforce。 活動（例如電子郵件和呼叫）會記錄到 [單向同步](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [取消訂閱數](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) 和 [提醒任務](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) 會以雙向同步方式保持最新。 這些資料同步都可從Sales Insight Actions網頁應用程式介面設定。

>[!MORELIKETHIS]
>
>* [將取消訂閱與Salesforce同步](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo取消訂閱檢查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Salesforce同步設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [與Salesforce的提醒任務同步](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [啟動資料同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

