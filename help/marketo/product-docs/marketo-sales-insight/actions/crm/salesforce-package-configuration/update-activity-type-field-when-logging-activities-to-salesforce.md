---
description: 將活動記錄到Salesforce時更新活動型別欄位 — Marketo檔案 — 產品檔案
title: 將活動記錄到Salesforce時更新活動型別欄位
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 1%

---

# 將活動記錄到Salesforce時更新活動型別欄位 {#update-activity-type-field-when-logging-activities-to-salesforce}

動作可以自動將您的電子郵件和通話活動同步至Salesforce以用於報告，並提高活動歷史記錄的可見度。 記錄活動時，請確定活動型別欄位已正確更新為電子郵件、電話或回覆，具體取決於要記錄的活動型別。

>[!NOTE]
>
>透過「密件副本」記錄電子郵件將不會檢視「任務型別」選擇清單，而是會自動將型別欄位填入為「電子郵件」，因為這些電子郵件會透過您的「密件副本」地址傳送給Salesforce。

## 須知 {#things-to-know}

* 必須與Salesforce建立連線，工作型別才能更新。
* 「工作型別」選擇清單上不應選取預設的「型別」值。
* 「工作型別」選擇清單中必須存在呼叫、回覆及電子郵件（大寫重要）。
* Salesforce中更新任務型別欄位的工作流程或觸發器可能會干擾此流程。

## 設定 {#setup}

首先檢查您是否已準備好正確的挑選清單值。 您需要Salesforce管理員的協助，才能對挑選清單進行任何變更。

首先檢查您的任務型別選擇清單（電子郵件、通話和回覆中）中缺少哪些值。 您可能需要Salesforce管理員的協助，才能檢閱此資訊，並變更活動型別選擇清單。 若要進行這些變更，您的Salesforce管理員可以依照下列步驟操作。

### 在Salesforce Lightning中 {#salesforce-lightning}

1. 瀏覽至[Salesforce.com](https://salesforce.com){target="_blank"}。
1. 按一下右上角的齒輪圖示，然後選取&#x200B;**設定** > **物件管理員**。
1. 在「快速尋找」方塊中輸入「任務」。
1. 在左側面板中，按一下&#x200B;**欄位和關係**。
1. 按一下欄位標籤&#x200B;**型別**。
1. 在工作型別選擇清單值下，按一下&#x200B;**新增**。
1. 輸入遺失的「任務型別」挑選清單值（「電子郵件」、「呼叫」、「回覆」）的名稱。
1. 按一下&#x200B;**保存**。

### 在Salesforce Classic中 {#salesforce-classic}

1. 瀏覽至[Salesforce.com](https://salesforce.com){target="_blank"}。
1. 按一下&#x200B;**設定** > **建置** > **自訂** > **活動** > **工作列位**。
1. 按一下&#x200B;**型別**。
1. 在工作型別選擇清單值下，按一下&#x200B;**新增**。
1. 輸入遺失的「任務型別」挑選清單值（「電子郵件」、「呼叫」、「回覆」）的名稱。
1. 按一下&#x200B;**保存**。

現在這項功能已就緒，您就會開始看到「型別」欄位填入記錄的電子郵件、來電和回覆的對應值。 這些值將&#x200B;_不會_&#x200B;填入銷售分析動作提醒任務中。

>[!NOTE]
>
>如果您沒有看到「回覆」的值，請按一下「新增」****&#x200B;以新增該值。 &#39;Reply&#39;不是Salesforce中的標準值。

>[!MORELIKETHIS]
>
>* [將銷售活動屬性記錄到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [設定Salesforce活動詳細資料自訂](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [將銷售活動同步至Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
