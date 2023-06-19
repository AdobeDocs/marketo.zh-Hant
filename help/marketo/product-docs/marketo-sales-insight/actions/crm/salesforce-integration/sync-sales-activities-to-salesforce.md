---
description: 將銷售活動同步至Salesforce - Marketo檔案 — 產品檔案
title: 將銷售活動同步至Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 將銷售活動同步至Salesforce {#sync-sales-activities-to-salesforce}

您可以設定Actions Salesforce同步設定來記錄電子郵件和呼叫Salesforce的活動。 這樣可讓團隊在您的CRM之外工作更清楚，並可讓經理使用這些活動來建立自訂Salesforce報告，以追蹤您的團隊績效。

## 透過API將電子郵件活動記錄到Salesforce {#logging-email-activity-to-salesforce-via-api}

若要使用此功能，您必須使用Enterprise/Unlimited版的Salesforce，或是Professional版（如果您已透過Web Services API購買整合）。

>[!PREREQUISITES]
>
>Salesforce與Sales Insight Actions必須連線。

1. 在銷售分析動作中，按一下齒輪圖示並選取 **設定**.

   ![](assets/sync-sales-activities-to-salesforce-1.png)

1. 在「管理員設定」（如果您不是管理員，則稱為「我的帳戶」）下，按一下 **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-2.png)

1. 按一下 **同步設定** 標籤。

   ![](assets/sync-sales-activities-to-salesforce-3.png)

1. 按一下「將電子郵件活動記錄到Salesforce」旁的箭頭。

   ![](assets/sync-sales-activities-to-salesforce-4.png)

1. 按一下 **Salesforce API** 標籤。 在此卡片中，您可以設定將資訊記錄到Salesforce的偏好設定。 按一下 **儲存** 完成時。

   ![](assets/sync-sales-activities-to-salesforce-5.png)

## 透過傳送電子郵件至Salesforce （密件副本），將電子郵件活動記錄到Salesforce {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

一旦您啟用「傳送電子郵件給Salesforce （密件副本）」，您將收到銷售電子郵件的密件副本，並且您的電子郵件將記錄為商機、潛在客戶和聯絡人的活動。

>[!PREREQUISITES]
>
>Salesforce與Sales Insight Actions必須連線。

**透過電子郵件（密件副本）在Salesforce中記錄您的電子郵件**

1. 在Marketo Sales中，按一下齒輪圖示並選取 **設定**.

   ![](assets/sync-sales-activities-to-salesforce-6.png)

1. 在「管理員設定」（如果您不是管理員，則稱為「我的帳戶」）下，按一下 **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-7.png)

1. 按一下 **同步設定** 標籤。

   ![](assets/sync-sales-activities-to-salesforce-8.png)

1. 按一下 **傳送電子郵件至Salesforce （密件副本）** 標籤並按一下 **啟動**.

   ![](assets/sync-sales-activities-to-salesforce-9.png)

如果由於某些原因，您的Email to Salesforce地址沒有拉入，請按照以下步驟在您的Salesforce帳戶中啟動密件副本功能：

1. 登入您的Salesforce執行個體。
1. 在右上角找到您的使用者名稱，然後選取下拉式清單。
1. 選取 **我的設定**.
1. 選取 **電子郵件**.
1. 選取 **我的電子郵件至Salesforce**.
1. 在此頁面中，您會看到標示為「傳送電子郵件至Salesforce位址」的欄位。 如果旁邊未填入任何內容，請向下捲動至「我的可接受電子郵件地址」。
1. 輸入您想要密件副本的電子郵件地址。
1. 按一下 **儲存變更**.

**在「我的設定」中找不到我的電子郵件給Salesforce**

如果您在「設定」底下沒有看到「我寄給Salesforce的電子郵件」，可能是因為您的管理員沒有啟用它。 如果您的團隊不熟悉Salesforce，或您的團隊從未使用Salesforce提供的密件副本地址，就可能發生這種情況。

>[!NOTE]
>
>您需要管理員許可權才能設定此專案。

1. 按一下 **設定**.
1. 按一下 **電子郵件管理**.
1. 按一下 **傳送電子郵件至Salesforce**.
1. 按一下 **編輯**.
1. 勾選「作用中」旁的方塊。
1. 按一下 **儲存**.

## 將Sales Insight Actions任務/提醒同步至Salesforce任務 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在銷售分析動作中，按一下齒輪圖示並選取 **設定**.

   ![](assets/sync-sales-activities-to-salesforce-10.png)

1. 在「管理員設定」（如果您不是管理員，則稱為「我的帳戶」）下，按一下 **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-11.png)

1. 按一下 **同步設定** 標籤。

   ![](assets/sync-sales-activities-to-salesforce-12.png)

1. 按一下「將Marketo銷售工作/提醒同步至Salesforce工作」旁的箭頭。

   ![](assets/sync-sales-activities-to-salesforce-13.png)

1. 選擇所需的選項（預設會選取「不要同步至Salesforce工作」）。

   ![](assets/sync-sales-activities-to-salesforce-14.png)

## 首次將Sales Insight動作任務與Salesforce同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Insight Actions與Salesforce任務之間的同步時，我們會匯入您的Salesforce任務。 我們不會將您在Sales Insight Actions中的任何目前任務推送到Salesforce。 為了減少雜湊和重複專案，從Sales Insight Actions同步至Salesforce的唯一工作是在您將Sales Insight Actions與SFDC同步後建立的工作。

以下是在同步Sales Insight Actions和SFDC任務時發生的情況：

* 當您在任務同步處理上按一下「儲存」時，它們就會開始進行同步處理。 這最初需要一些時間。

* 過去24小時內已更新或建立的任何提醒都會從SFDC提取至Sales Insight動作。 同步是根據到期日，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天的到期工作。

* 如果先前已開啟同步處理，而您刪除了SFDC中的任何工作，則過去15天內刪除的任何工作都將從指揮中心刪除。

* 只要同步功能已啟用，我們就會持續在Sales Insight Actions與SFDC之間同步工作。

* 初次同步後，您在Sales Insight Actions中建立、編輯、完成或刪除的任何任務都會同步至您在Salesforce中的任務清單。 在Salesforce中建立、編輯、完成或刪除的任何專案，都會更新Sales Insight Actions中的任務清單。

* 若要開啟此同步，只要勾選Web應用程式中「設定」頁面中的同步方塊即可。
