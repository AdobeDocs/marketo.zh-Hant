---
description: Salesforce同步設定 — Marketo文檔 — 產品文檔
title: Salesforce同步設定
hide: true
hidefromtoc: true
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: acb077e9d6e9fa4027d660ee182a13820f16ad83
workflow-type: tm+mt
source-wordcount: '443'
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
