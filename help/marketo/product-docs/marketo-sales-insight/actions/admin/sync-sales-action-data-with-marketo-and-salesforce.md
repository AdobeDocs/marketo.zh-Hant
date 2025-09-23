---
description: 將銷售動作資料與Marketo和Salesforce同步 — Marketo檔案 — 產品檔案
title: 與 Marketo 和 Salesforce 同步銷售動作資料
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 3%

---

# 與 Marketo 和 Salesforce 同步銷售動作資料 {#sync-sales-action-data-with-marketo-and-salesforce}

Sales Insight Actions的資料統一欄位同步可讓系統從Marketo Engage資料庫將人員資訊提取到Sales Insight Actions資料庫中。

如此可在Sales Insight Actions網頁應用程式中提供最新的人員資料，並允許系統收集Marketo中對應人員記錄的唯一ID以及Salesforce中的銷售機會/聯絡人/帳戶/機會記錄，以便能夠正確參考記錄以記錄資料。

此同步可從Marketo Engage的「管理員」區段中的「銷售Insight動作設定」標籤啟用。 如需詳細資訊，請參閱[啟動資料同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)。

![](assets/actions-data-sync-faq-1.png)

上圖顯示人員活動和任務資料如何在系統之間同步。 請注意下列事項：

* 人員記錄會同步至Marketo Engage的Sales Insight Actions，讓Marketo Engage成為Sales Insight Actions人員資料的真實來源
* Marketo Engage和Sales Insight動作[都有收集取消訂閱狀態並將其同步至Salesforce的機制](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
* 取消訂閱狀態不會從銷售動作同步到Marketo Engage，但銷售Insight動作可以設定為先檢查人員的Marketo取消訂閱狀態，然後再允許賣家傳送包含[Marketo取消訂閱檢查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)的電子郵件。

以下是與資料統一同步如何運作相關的一些常見問題。

## 哪些銷售機會/聯絡人會同步至「銷售Insight動作」？ {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

已指定銷售負責人的潛在客戶與聯絡人會同步至「銷售作業」。

您可以檢視現有的標準擁有者欄位，瞭解銷售機會/聯絡人在Salesforce中是否有銷售擁有者。

銷售擁有者不必是Marketo同步使用者或任何特定的Salesforce或銷售使用者。 我們只需在Salesforce中列出的潛在客戶擁有者和聯絡人擁有者欄位中列出使用者，我們就能將其識別為銷售潛在客戶，並將其同步至Sales Insight Actions。 與我們同步之欄位的任何更新也會在Sales Insight動作中偵測及更新。

## Sales Insight Smart Grid中顯示的活動資料來自何處？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

電子郵件、電話、有趣的時刻和網頁等活動資料都來自Marketo Engage的資料庫。 Sales Insight Smart Grid會在每次銷售使用者載入Sales Insight面板時，向Marketo Engage執行個體提出擷取此內容的請求。

![](assets/actions-data-sync-faq-4.png)

為確保所有活動資料皆可從Marketo Engage取得，Sales Insight Actions會將所有活動資料同步至Marketo Engage。

## 哪些欄位與從Marketo Engage同步至銷售Insight動作的人員記錄有關？ {#what-fields-sync}

有11個欄位會從Marketo Engage同步至銷售Insight動作：

* 名字
* 姓氏
* Salesforce聯絡人ID
* Salesforce銷售機會ID
* Salesforce帳戶ID
* Salesforce機會ID
* Marketo ID
* 公司
* 標題
* 電子郵件
* 電話號碼
* Linkedin URL
* 來源

## 在Marketo Engage和Sales Insight Actions之間同步的欄位是否可設定？ {#are-the-fields-that-sync-configurable}

無法設定同步至銷售Insight動作的Marketo Engage欄位，也無法對應欄位。 來自Marketo的同步會自動將標準Marketo欄位對應到銷售動作例項中的標準欄位。

## 為什麼銷售Insight Actions有自己的資料庫？ {#why-does-actions-have-its-own-database}

Sales Insight Actions有自己的網頁應用程式，其中包含專屬的人員與活動資料庫，可提供專為銷售團隊建立及設計的最佳化工作區。 這可讓銷售經理和銷售商有空間建立和管理他們的參與策略   無需授與主要Marketo Engage工作區的存取權或許可權，此工作區已針對行銷作業專家最佳化。

## 如何處理重複專案？ {#how-are-duplicates-handled}

您的Sales Actions資料庫將是存在於Marketo Engage資料庫中之合格人員（具有銷售負責人的銷售機會/聯絡人）的副本。 也就是說，如果在Marketo中建立了兩個具有相同電子郵件地址的記錄，則在「銷售動作」中將會建立重複的記錄。

## 初始同步處理需要多久的時間才能完成？ {#how-long-initial-sync}

將所有銷售機會資料同步至新的Sales Insight Actions例項的初始程式，通常每1-2分鐘會處理約1,000名人員。 這只是估計值，可能會有所不同。

一旦進行初始同步且您的所有銷售機會已填入您的Sales Insight Actions網頁應用程式執行個體後，每次更新已同步的支援欄位之一時，就會執行增量同步。

## Sales Insight Actions使用者是否可從Actions Web應用程式編輯人員資料？ {#can-actions-users-edit-people-data}

否，「動作」網頁應用程式的使用者和管理員都無法在「動作」中建立及編輯人員記錄。 必須在Salesforce或Marketo Engage中建立和編輯人員。 Sales Insight Actions會持續同步新資料，以使用Marketo作為人員資料的信任來源，因此，如果在Marketo中從Marketo的工作流程更新或建立人員，或是從Salesforce同步人員，這些更新都會傳遞至Sales Insight Actions Web應用程式資料庫。

## 銷售活動會記錄到Marketo嗎？ {#do-sales-activities-log-to-marketo}

是，銷售參與活動會以原生活動的形式登入Marketo。 這些活動也包含原生篩選器，可搭配條件約束使用，以根據銷售活動屬性來鎖定潛在客戶。

![](assets/actions-data-sync-faq-5.png)

以下是登入Marketo的活動清單：

* 傳送銷售電子郵件
* 開啟銷售電子郵件
* 點按銷售電子郵件
* 已回覆銷售電子郵件
* 銷售電子郵件已退回
* 已接聽銷售電話
* 新增至銷售行銷活動
* 已從銷售行銷活動中移除

## 銷售活動會記錄到Salesforce嗎？ {#do-sales-activities-log-to-salesforce}

是，銷售參與活動會以原生工作的形式登入Salesforce。 這些工作隨後可用於Salesforce報表，以支援追蹤銷售活動的團隊儀表板。

銷售Insight動作可讓管理員設定哪些銷售活動記錄到Salesforce。 這些活動包括電子郵件、來電和開啟提醒工作。

![](assets/actions-data-sync-faq-6.png)

上圖顯示哪些資訊會記錄到Salesforce。 電子郵件和通話等活動會以[單向同步](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)記錄到Salesforce。 [取消訂閱](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)與[提醒工作](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)會以雙向同步方式保持最新狀態。 這些資料同步可從Sales Insight Actions網頁應用程式介面設定。

>[!MORELIKETHIS]
>
>* [正在與Salesforce同步取消訂閱](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo取消訂閱檢查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [將銷售活動同步至Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [提醒工作與Salesforce同步](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [啟動資料同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
