---
description: 將活動記錄到Salesforce時更新活動型別欄位 — Marketo檔案 — 產品檔案
title: 將活動記錄到Salesforce時更新活動型別欄位
source-git-commit: 46c48172a58cf6bd2e9772ef57510fd7d808adc2
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# 將活動記錄到Salesforce時更新活動型別欄位 {#update-activity-type-field-when-logging-activities-to-salesforce}

動作可以自動將您的電子郵件和通話活動同步至Salesforce以用於報告，並提高活動歷史記錄的可見度。 記錄活動時，請確定活動型別欄位已正確更新為電子郵件、通話或回覆，具體取決於所記錄的活動型別。

>[!NOTE]
>
>透過「密件副本」記錄電子郵件不會檢視「任務型別」選擇清單，而是會自動將「型別」欄位填入為「電子郵件」，因為這些電子郵件會透過您的「密件副本」地址傳送到Salesforce。

## 須知事項 {#things-to-know}

* 必須與Salesforce建立連線，任務型別才能更新。
* 「任務型別」選擇清單上不應選取預設型別值。
* 「工作型別」選擇清單中必須有「通話」、「回覆」和「電子郵件」（大寫內容）。
* Salesforce中更新任務型別欄位的工作流程或觸發器可能會干擾此流程。

## 設定 {#setup}

首先檢查您是否有正確的挑選清單值。 您需要Salesforce管理員的協助，才能對挑選清單進行任何變更。

首先檢查您的任務型別選擇清單（來自電子郵件、通話和回覆）中缺少哪些值。 您可能需要Salesforce管理員的協助，才能檢閱此資訊，並變更活動型別選擇清單。 若要進行這些變更，您的Salesforce管理員可以依照下列步驟進行。

### Salesforce Lightning內容 {#salesforce-lightning}

1. 導覽至 [Salesforce.com](https://salesforce.com){target="_blank"}.
1. 按一下右上角的齒輪圖示並選取 **設定** > **物件管理員**.
1. 在「快速尋找」方塊中輸入「任務」。
1. 在左側面板中，按一下 **欄位和關係**.
1. 按一下欄位標籤 **型別**.
1. 在任務型別選擇清單值下，按一下 **新增**.
1. 輸入遺失的「任務型別」挑選清單值的名稱（「電子郵件」、「呼叫」、「回覆」）。
1. 按一下 **儲存**.

### 在Salesforce Classic中 {#salesforce-classic}

1. 導覽至 [Salesforce.com](https://salesforce.com){target="_blank"}.
1. 按一下 **設定** > **建置** > **自訂** > **活動** > **工作列位**.
1. 按一下 **型別**.
1. 在任務型別選擇清單值下，按一下 **新增**.
1. 輸入遺失的「任務型別」挑選清單值的名稱（「電子郵件」、「呼叫」、「回覆」）。
1. 按一下 **儲存**.

完成設定後，您就會開始看到「型別」欄位填入記錄電子郵件、來電和回覆的對應值。 這些值將 _not_ 填入至銷售分析動作提醒任務中。

>[!NOTE]
>
>如果您沒有看到「回覆」值，請按一下以新增該值 **新增**. &#39;Reply&#39;不是Salesforce中的標準值。

>[!MORELIKETHIS]
>
>* [將銷售活動屬性記錄到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [設定Salesforce活動詳細資料自訂](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Salesforce同步設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md){target="_blank"}
