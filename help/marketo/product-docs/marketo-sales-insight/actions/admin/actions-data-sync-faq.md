---
description: 操作資料同步常見問題 — Marketo文檔 — 產品文檔
title: 操作資料同步常見問題
hide: true
hidefromtoc: true
source-git-commit: bde1c5487de349b9d01105a1cee28598f2d6a36c
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 0%

---

# 操作資料同步常見問題 {#actions-data-sync-faq}

Sales Insight Actions的資料統一欄位同步使系統能夠將人員資訊從您的Marketo Engage資料庫拉入您的Sales Insight Actions資料庫。

這可以在Sales Insight Actions Web應用中提供最新的人員資料，並允許系統為Marketo的相應人員記錄和Salesforce中的潛在客戶/聯繫人/帳戶/機會記錄收集唯一的ID，以便記錄可以被正確引用以記錄資料。

可以從Marketo Engage的「管理」部分的「Sales Insight Actions Config」（Sales Insight操作配置）頁籤啟用此同步。 有關詳細資訊，請簽出 [啟動資料同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/msi-actions-admin-guide.md#initiate-data-sync)。

![](assets/actions-data-sync-faq-1.png)

上圖顯示了人員活動和任務資料如何在系統之間同步。 需要注意的幾點：

* 人員記錄將從Marketo Engage同步到Sales Insight Actions，使Marketo Engage成為Sales Insight Actions人員資料的真相來源
* Marketo Engage和Sales Insight操作 [有一個機構](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) 用於收集和同步取消訂閱狀態到Salesforce
* 取消訂閱狀態不會從銷售活動同步到Marketo Engage，但可以將Sales Insight Actions配置為在允許銷售者發送電子郵件之前檢查人員的Marketo取消訂閱狀態 [Marketo取消訂閱支票](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)。

下面是一些與資料統一同步如何工作有關的常見問題。

## 哪些潛在客戶/聯繫人已同步到Sales Insight Actions? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

分配了銷售責任人的銷售線索和聯繫人將同步到銷售活動中。

通過查看現有的標準責任人欄位，您可以查看潛在顧客/聯繫人是否在Salesforce中擁有銷售責任人。

銷售所有者不必是Marketo同步用戶或任何特定的Salesforce或銷售用戶。 只要標準所有者欄位中列有用戶，我們將包括要同步到銷售活動的潛在顧客/聯繫人，並將其包括在要同步到該潛在顧客的同步欄位的任何更新中。

## Sales Insight Smart Grid中顯示的活動資料從何處獲得來源？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

活動資料，如電子郵件、呼叫、有趣的時刻和web，都是從Marketo Engage的資料庫中提取的。 Sales Insight Smart Grid向Marketo Engage實例發出請求，以在每次銷售用戶載入Sales Insight面板時檢索此實例。

![](assets/actions-data-sync-faq-4.png)

為確保所有活動資料都可以從Marketo Engage中補充，Oracle Sales Insight Actions會將所有活動資料同步到Marketo Engage。

## 與人員記錄相關的哪些欄位從Marketo Engage同步到Sales Insight操作？ {#what-fields-sync}

有11個欄位從Marketo Engage同步到Sales Insight操作：

* 名字
* 姓氏
* Salesforce聯繫人ID
* Salesforce潛在顧客ID
* MarketoID
* 公司
* 標題
* 電子郵件
* 電話號碼
* 林克丁URL
* 來源

## 在Marketo Engage和Sales Insight Actions之間同步的欄位是否可配置？ {#are-the-fields-that-sync-configurable}

配置與Sales Insight Actions同步的Marketo Engage欄位不可用，也不能映射欄位。 來自Marketo的同步會自動將標準Marketo欄位映射到您的銷售活動實例中的標準欄位。

## 為什麼Sales Insight Actions有自己的資料庫？ {#why-does-actions-have-its-own-database}

Sales Insight Actions有其自己的Web應用程式，並配備了專用的人員和活動資料庫，以提供為銷售團隊構建和設計的優化工作區。 這使銷售經理和銷售人員有空間構建和管理他們的接洽策略，而不授予對主要Marketo Engage工作區的訪問權限或權限，而主要銷售工作區是為市場營銷操作專家而優化的。

## 如何處理重複項？ {#how-are-duplicates-handled}

您的Sales Actions資料庫將是Marketo Engage資料庫中存在的那些合格人員（銷售負責人的銷售線索/聯繫人）的副本。 這意味著，如果在Marketo建立了兩個具有相同電子郵件地址的記錄，則在「銷售操作」中將建立重複的記錄。

## 完成初始同步需要多長時間？ {#how-long-initial-sync}

將所有銷售線索資料同步到新Sales Insight Actions實例的初始過程通常每1-2分鐘處理1,000人。 這只是一個估計，可能有所不同。

一旦初始同步發生，並且您的所有銷售線索都已填充到您的Sales Insight Actions Web應用實例中，則每次更新某個同步的受支援欄位時都會運行增量同步。

## Sales Insight Actions用戶是否可以編輯Actions Web應用中的人員資料？ {#can-actions-users-edit-people-data}

否，在「操作」中建立和編輯人員記錄的功能對Actions Web應用的用戶和管理員都不可用。 必須在Salesforce或Marketo Engage中建立和編輯人員。 Sales Insight Actions通過持續同步新資料將Marketo用作人員資料的真相來源，因此，如果在Marketo更新或建立人員是從Marketo的工作流或從Salesforce同步的，則這些更新將傳遞到Sales Insight Actions Web應用資料庫。

## 銷售活動是否記錄到Marketo? {#do-sales-activities-log-to-marketo}

是的，銷售參與活動將作為本地活動登錄Marketo。 這些活動還包括本機篩選器，這些篩選器可與基於銷售活動屬性的目標銷售線索的約束一起使用。

![](assets/actions-data-sync-faq-5.png)

以下是登錄Marketo的活動清單：

* 發送銷售電子郵件
* 開啟銷售電子郵件
* 按一下銷售電子郵件
* 已回復銷售電子郵件
* 銷售電子郵件已退出
* 已接收銷售呼叫
* 添加到銷售活動
* 從銷售活動中刪除

## 銷售活動是否記錄到Salesforce? {#do-sales-activities-log-to-salesforce}

是的，銷售參與活動將作為本機任務登錄到Salesforce。 然後，這些任務可以在Salesforce報表中使用，以為跟蹤銷售活動的團隊控制板提供動力。

Sales Insight Actions允許管理員配置哪些銷售活動記錄到Salesforce。 這些活動包括電子郵件、呼叫和未結提醒任務。

![](assets/actions-data-sync-faq-6.png)

上圖顯示了哪些資訊記錄到Salesforce。 電子郵件和呼叫等活動將記錄到Salesforce中 [單向同步](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)。 [取消訂閱](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) 和 [提醒任務](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) 通過雙向同步保持最新。 每個資料同步都可從Sales Insight Actions Web app介面進行配置。

>[!MORELIKETHIS]
>
>* [正在與Salesforce同步取消訂閱](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo取消訂閱支票](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Salesforce同步設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [提醒任務與Salesforce同步](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)

