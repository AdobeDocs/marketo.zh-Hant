---
description: 為什麼我的銷售活動和活動欄位未同步至Salesforce？ - Marketo檔案 — 產品檔案
title: 為什麼我的銷售活動和活動欄位未同步至Salesforce？
source-git-commit: c50f0f08914076a440026fb368bf38763b282bbf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 為什麼我的銷售活動和活動欄位未同步至Salesforce？ {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**我看不到電子郵件或通話活動同步至Salesforce。**

* 確定您已連線至Salesforce。 每位使用者都需要連線以記錄其對Salesforce的電子郵件和通話。
* 請確定您已設定 [Salesforce同步設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* 電子郵件會根據Salesforce ID作為主要查詢，並根據Email Address作為次要查詢來進行記錄查詢。 您可以確認人員記錄在「 」中連結了Salesforce ID和電子郵件地址 [動作Web應用程式](https://toutapp.com/next#command_center){target="_blank"}.
* 呼叫只會根據Salesforce ID執行記錄查閱。 如果「動作」中的人員記錄上不存在Salesforce ID，呼叫將不會記錄。 您可以確認人員記錄在「 」中連結至他們的Salesforce ID [動作Web應用程式](https://toutapp.com/next#command_center){target="_blank"}.

**我沒有在Salesforce更新中看到活動欄位。**

如果您沒有看到電子郵件 [活動屬性欄位](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} 在Salesforce中更新，可能是因為您團隊的欄位可存取性受限。 Salesforce欄位層級安全性讓Salesforce管理員能夠限制使用者可檢視和編輯的資訊。 如果「動作」使用者無權檢視及編輯這些欄位，「動作」活動同步將無法更新這些欄位。

* 請與您的Salesforce管理員合作，確保這些安全性設定不會受到干擾 [Actions Salesforce活動欄位](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* 如果您是Salesforce管理員，可以在「安全性控制」標籤下看到您的欄位可存取性。 與「作業」互動的主要物件包括：銷售機會、聯絡人、帳戶、商機及作業/作業。

>[!NOTE]
>
>與Lead 、 Contact 、 Account和Opportunity物件相關聯的欄位將隨Sales Insight Salesforce套件一起安裝。 與關聯的欄位 [需要建立任務/活動記錄型別](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} 由Salesforce管理員提供。
