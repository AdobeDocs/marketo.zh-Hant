---
description: 我的銷售活動和活動欄位為何未同步至Salesforce？ - Marketo檔案 — 產品檔案
title: 我的銷售活動和活動欄位為何未同步至Salesforce？
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 我的銷售活動和活動欄位為何未同步至Salesforce？ {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**我沒有看到同步至Salesforce的電子郵件或通話活動。**

* 請確定您已連線至Salesforce。 每位使用者都必須有連線，才能記錄其傳送至Salesforce的電子郵件和電話。
* 確定您已設定[Salesforce同步設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}。
* 電子郵件會根據Salesforce ID來執行記錄查詢，以作為主要查詢，而電子郵件地址會作為次要查詢。 您可以在[Actions網頁應用程式](https://toutapp.com/next#command_center){target="_blank"}中確認個人記錄具有連結至他們的Salesforce ID和電子郵件地址。
* 呼叫只會根據Salesforce ID執行記錄查詢。 如果「動作」中的人員記錄上不存在Salesforce ID，則不會記錄呼叫。 您可以在[動作網頁應用程式](https://toutapp.com/next#command_center){target="_blank"}中確認個人記錄具有連結至他們的Salesforce ID。

**我沒有在Salesforce更新中看到活動欄位。**

如果您在Salesforce中未看到電子郵件[活動屬性欄位](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}更新，可能是因為您團隊的欄位可存取性有所限制。 Salesforce欄位層級安全性讓Salesforce管理員能夠限制使用者可檢視和編輯的資訊。 如果「動作」使用者無權檢視及編輯這些欄位，「動作」活動同步將無法更新這些欄位。

* 請與您的Salesforce管理員合作，確保這些安全性設定不會干擾[動作Salesforce活動欄位](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
* 如果您是Salesforce管理員，可以在「安全性控制」標籤下看到您的欄位可存取性。 與「作業」互動的主要物件有：銷售機會、聯絡人、科目、商機及作業/作業。

>[!NOTE]
>
>與Lead、Contact、Account和Opportunity物件相關聯的欄位將與Sales Insight Salesforce套件一起安裝。 與[任務/活動記錄型別相關聯的欄位需要由Salesforce管理員建立](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}。
