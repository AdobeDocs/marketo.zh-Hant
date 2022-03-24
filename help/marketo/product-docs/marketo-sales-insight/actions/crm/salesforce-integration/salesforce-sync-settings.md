---
description: Salesforce同步設定 — Marketo文檔 — 產品文檔
title: Salesforce同步設定
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Salesforce同步設定 {#salesforce-sync-settings}

## 通過API將電子郵件活動記錄到Salesforce {#logging-email-activity-to-salesforce-via-api}

此功能要求您在Salesforce的Enterprise/Unlimited版本上，或者如果您已通過Web Services API購買了Integration，則必須在Professional版本上。

>[!PREREQUISITES]
>
>必須連接Salesforce和Sales Insight Actions。

1. 在Sales Insight Actions中，按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/salesforce-sync-settings-1.png)

1. 在「管理員設定」（如果您不是管理員，請按一下「我的帳戶」）下 **Salesforce**。

   ![](assets/salesforce-sync-settings-2.png)

1. 按一下 **同步設定** 頁籤。

   ![](assets/salesforce-sync-settings-3.png)

1. 按一下「將電子郵件活動記錄到Salesforce」旁邊的箭頭。

   ![](assets/salesforce-sync-settings-4.png)

1. 按一下 **Salesforce API** 頁籤。 在此卡中，您可以設定您對將資訊記錄到Salesforce的首選項。 按一下 **保存** 完成。

   ![](assets/salesforce-sync-settings-5.png)

## 通過電子郵件將電子郵件活動記錄到Salesforce(BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

一旦激活「向Salesforce(BCC)發送電子郵件」，您將收到一份BCC的銷售電子郵件，您的電子郵件將作為有關業務機會、銷售線索和聯繫人的活動記錄。

>[!PREREQUISITES]
>
>必須連接Salesforce和Sales Insight Actions。

**通過電子郵件（密件抄送）在Salesforce中記錄電子郵件**

1. 在「Marketo銷售」中，按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/salesforce-sync-settings-6.png)

1. 在「管理員設定」（如果您不是管理員，請按一下「我的帳戶」）下 **Salesforce**。

   ![](assets/salesforce-sync-settings-7.png)

1. 按一下 **同步設定** 頁籤。

   ![](assets/salesforce-sync-settings-8.png)

1. 按一下 **電子郵件至Salesforce(BCC)** 頁籤 **激活**。

   ![](assets/salesforce-sync-settings-9.png)

如果由於某種原因您的E-Mail to Salesforce地址未加入，請按照以下步驟在您的Salesforce帳戶中激活BCC功能：

1. 登錄到Salesforce實例。
1. 在右上角查找您的用戶名並選擇下拉條。
1. 選擇 **我的設定**。
1. 選擇 **電子郵件**。
1. 選擇 **我給Salesforce的電子郵件**。
1. 在此頁上，您將看到一個標有「E-mail to Salesforce Address（向Salesforce地址發送電子郵件）」的欄位。 如果旁邊沒有填充內容，請向下滾動到「My Accepted E-mail Addresses（我可接受的電子郵件地址）」。
1. 輸入要BCC的電子郵件地址。
1. 按一下 **保存更改**。

**在「我的設定」中找不到我的電子郵件至Salesforce**

如果您在「設定」下未看到「我向Salesforce發送電子郵件」，則您的管理員可能未啟用它。 如果您的團隊是Salesforce的新成員，或者您的團隊從未使用Salesforce提供的BCC地址，則可能會發生這種情況。

>[!NOTE]
>
>您需要管理員權限才能設定。

1. 按一下 **設定**。
1. 按一下 **電子郵件管理**。
1. 按一下 **電子郵件至Salesforce**。
1. 按一下 **編輯**。
1. 選中「Active（活動）」旁邊的框。
1. 按一下 **保存**。

## 將Sales Insight操作任務/提醒同步到Salesforce任務 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在Sales Insight Actions中，按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/salesforce-sync-settings-10.png)

1. 在「管理員設定」（如果您不是管理員，請按一下「我的帳戶」）下 **Salesforce**。

   ![](assets/salesforce-sync-settings-11.png)

1. 按一下 **同步設定** 頁籤。

   ![](assets/salesforce-sync-settings-12.png)

1. 按一下「將Marketo銷售任務/提醒同步到Salesforce任務」旁邊的箭頭。

   ![](assets/salesforce-sync-settings-13.png)

1. 選擇所需選項（預設情況下選擇「不同步到Salesforce任務」）。

   ![](assets/salesforce-sync-settings-14.png)

## 首次將Sales Insight Actions任務與Salesforce同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

當您首次啟用Sales Insight Actions和Salesforce任務之間的同步時，我們將導入您的Salesforce任務。 我們不會將您在Sales Insight Actions中擁有的任何當前任務推送到Salesforce。 為減少雜亂和重複，從Sales Insight Actions同步到Salesforce的任務只有在將Sales Insight Actions與SFDC同步後建立的任務。

以下是同步Sales Insight Actions和SFDC任務時發生的情況：

一旦按一下「保存任務」同步，它們就開始同步。 這需要一些時間。

在過去24小時內更新或建立的任何提醒都將從SFDC拉入到Sales Insight Actions。 同步基於到期日期，所有這些任務都將在後端進行同步，但在命令中心中，您將只看到今天和明天到期的任務。

如果以前已啟用同步並且您刪除了SFDC中的任何任務，則在過去15天內刪除的任何任務都將從命令中心刪除。

只要啟用同步，我們就會在Sales Insight Actions和SFDC之間不斷同步任務。

在初始同步後，您在Sales Insight Actions中建立、編輯、完成或刪除的任何任務都將同步到Salesforce中的任務清單。 任何在Salesforce中建立、編輯、完成或刪除的內容都將更新Sales Insight Actions中的任務清單。

要啟用此同步，只需選中Web應用程式的「設定」頁中的同步框。
