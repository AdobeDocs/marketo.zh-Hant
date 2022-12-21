---
description: Salesforce同步設定 — Marketo檔案 — 產品檔案
title: Salesforce同步設定
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Salesforce同步設定 {#salesforce-sync-settings}

## 透過API將電子郵件活動記錄至Salesforce {#logging-email-activity-to-salesforce-via-api}

若您已透過網站服務API購買整合，則需要使用Salesforce的企業版/不限數量版，或專業版。

>[!PREREQUISITES]
>
>必須連接Salesforce和Sales Insight Actions。

1. 在Sales Insight Actions中，按一下齒輪圖示並選取 **設定**.

   ![](assets/salesforce-sync-settings-1.png)

1. 在「管理員設定」(或「我的帳戶」（如果您不是管理員）下，按一下 **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. 按一下 **同步設定** 標籤。

   ![](assets/salesforce-sync-settings-3.png)

1. 按一下「將電子郵件活動記錄到Salesforce」旁的箭頭。

   ![](assets/salesforce-sync-settings-4.png)

1. 按一下 **Salesforce API** 標籤。 在此卡中，您可以設定您對於將資訊記錄到Salesforce的首選項。 按一下 **儲存** 時才能使用。

   ![](assets/salesforce-sync-settings-5.png)

## 透過電子郵件將電子郵件活動記錄到Salesforce(BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活「Email to Salesforce(BCC)」後，您將收到銷售電子郵件的BCC，並且您的電子郵件將作為有關機會、銷售機會和聯繫人的活動進行記錄。

>[!PREREQUISITES]
>
>必須連接Salesforce和Sales Insight Actions。

**若要透過電子郵件(BCC)在Salesforce中記錄您的電子郵件**

1. 在「Marketo銷售」中，按一下齒輪圖示並選取 **設定**.

   ![](assets/salesforce-sync-settings-6.png)

1. 在「管理員設定」(或「我的帳戶」（如果您不是管理員）下，按一下 **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. 按一下 **同步設定** 標籤。

   ![](assets/salesforce-sync-settings-8.png)

1. 按一下 **發送電子郵件至Salesforce(BCC)** 按一下 **啟動**.

   ![](assets/salesforce-sync-settings-9.png)

如果由於某些原因，您的致Salesforce的電子郵件地址未被提取，請按照下列步驟在您的Salesforce帳戶中啟用BCC功能：

1. 登入您的Salesforce例項。
1. 在右上角找到您的使用者名稱，然後選取下拉式清單列。
1. 選擇 **我的設定**.
1. 選擇 **電子郵件**.
1. 選擇 **我給Salesforce的電子郵件**.
1. 在此頁面上，您會看到標示為「Email to Salesforce Address」的欄位。 如果旁邊未填入任何項目，請向下捲動至「我可接受的電子郵件地址」。
1. 輸入要BCC的電子郵件地址。
1. 按一下 **儲存變更**.

**在我的設定中找不到我給Salesforce的電子郵件**

如果您的「設定」下沒有看到「我給Salesforce的電子郵件」，則您的管理員可能尚未啟用它。 如果您的團隊是Salesforce的新手，或您的團隊從未使用Salesforce提供的BCC地址，就會發生此情況。

>[!NOTE]
>
>您需要管理員權限才能設定此設定。

1. 按一下 **設定**.
1. 按一下 **電子郵件管理**.
1. 按一下 **發送電子郵件給Salesforce**.
1. 按一下 **編輯**.
1. 勾選「作用中」旁的方塊。
1. 按一下 **儲存**.

## 同步Sales Insight操作任務/提醒至Salesforce任務 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在Sales Insight Actions中，按一下齒輪圖示並選取 **設定**.

   ![](assets/salesforce-sync-settings-10.png)

1. 在「管理員設定」(或「我的帳戶」（如果您不是管理員）下，按一下 **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. 按一下 **同步設定** 標籤。

   ![](assets/salesforce-sync-settings-12.png)

1. 按一下「同步Marketo銷售任務/提醒至Salesforce任務」旁邊的箭頭。

   ![](assets/salesforce-sync-settings-13.png)

1. 選擇所需的選項（預設會選取「不同步至Salesforce任務」）。

   ![](assets/salesforce-sync-settings-14.png)

## 首次將Sales Insight活動任務與Salesforce同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

當您首次開啟Sales Insight Actions和Salesforce任務之間的同步時，我們會導入您的Salesforce任務。 我們不會將您在Sales Insight Actions中擁有的任何當前任務推送到Salesforce。 為了減少雜亂和重複，從Sales Insight Actions同步到Salesforce的任務只有在您將Sales Insight Actions與SFDC同步後建立的任務。

以下是同步Sales Insight Actions和SFDC任務時會發生的情況：

當您按一下「儲存」時，即會開始同步工作。 這需要一些時間。

在過去24小時內更新或建立的任何提醒都將從SFDC提取到Sales Insight Actions。 同步基於到期日，所有這些任務都將在後端同步，但在命令中心，您將只看到今天和明天的任務。

如果以前已開啟同步，而您刪除了SFDC中的任何任務，則在過去15天中被刪除的任何任務都將從命令中心中刪除。

只要啟用同步，我們就會在Sales Insight Actions和SFDC之間不斷同步任務。

初始同步後，您在Sales Insight Actions中建立、編輯、完成或刪除的任何任務都將同步到Salesforce中的任務清單。 而任何在Salesforce中建立、編輯、完成或刪除的項目，都會在Sales Insight Actions中更新您的任務清單。

若要開啟此同步，只要勾選Web應用程式中「設定」頁面中的同步方塊即可。
