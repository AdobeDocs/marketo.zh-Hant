---
description: Salesforce同步設定 — Marketo檔案 — 產品檔案
title: Salesforce同步設定
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# [!DNL Salesforce]同步設定 {#salesforce-sync-settings}

## 透過API將電子郵件活動記錄到[!DNL Salesforce] {#logging-email-activity-to-salesforce-via-api}

若要使用此功能，您必須使用[!DNL Salesforce]的Enterprise/Unlimited版本，或是Professional版本（如果您已透過Web Services API購買整合）。

>[!PREREQUISITES]
>
>[!DNL Salesforce]與[!DNL Sales Insight Actions]必須連線。

1. 在[!DNL Sales Insight Actions]中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-sync-settings-1.png)

1. 在「[!UICONTROL Admin Settings]」下（如果您不是管理員，則按「[!UICONTROL My Account]」），按一下「**[!UICONTROL Salesforce]**」。

   ![](assets/salesforce-sync-settings-2.png)

1. 按一下「**[!UICONTROL Sync Settings]**」標籤。

   ![](assets/salesforce-sync-settings-3.png)

1. 按一下[!UICONTROL Log Email Activity]到[!DNL Salesforce]旁的箭頭。

   ![](assets/salesforce-sync-settings-4.png)

1. 按一下「**[!UICONTROL Salesforce API]**」標籤。 在此卡片中，您可以設定將資訊記錄到[!DNL Salesforce]的偏好設定。 完成時，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/salesforce-sync-settings-5.png)

## 透過電子郵件將電子郵件活動記錄到[!DNL Salesforce]至[!DNL Salesforce] （密件副本） {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

啟動「[!UICONTROL Email to Salesforce (BCC)]」後，您將會收到銷售電子郵件的密件副本，且您的電子郵件會記錄為商機、潛在客戶及聯絡人的活動。

>[!PREREQUISITES]
>
>[!DNL Salesforce]與[!DNL Sales Insight Actions]必須連線。

**透過電子郵件（密件副本）將您的電子郵件記錄在[!DNL Salesforce]**

1. 在Marketo銷售中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-sync-settings-6.png)

1. 在「[!UICONTROL Admin Settings]」下（如果您不是管理員，則按「[!UICONTROL My Account]」），按一下「**[!UICONTROL Salesforce]**」。

   ![](assets/salesforce-sync-settings-7.png)

1. 按一下「**[!UICONTROL Sync Settings]**」標籤。

   ![](assets/salesforce-sync-settings-8.png)

1. 按一下「**[!UICONTROL Email to Salesforce (BCC)]**」標籤，然後按一下「**[!UICONTROL Activate]**」。

   ![](assets/salesforce-sync-settings-9.png)

如果由於某種原因您的電子郵件至[!DNL Salesforce]位址沒有拉入，請依照下列步驟在您的[!DNL Salesforce]帳戶中啟動密件副本功能：

1. 登入您的[!DNL Salesforce]執行個體。
1. 在右上角找到您的使用者名稱，然後選取下拉式清單。
1. 選擇「**[!UICONTROL My Settings]**」。
1. 選擇「**[!UICONTROL Email]**」。
1. 選擇「**[!UICONTROL My Email to Salesforce]**」。
1. 在此頁面中，您會看到標示為「[!UICONTROL Email to Salesforce Address]」的欄位。 如果旁邊未填入任何內容，請向下捲動至&quot;[!UICONTROL My Acceptable Email Addresses]&quot;。
1. 輸入您要密件副本的電子郵件地址。
1. 按一下「**[!UICONTROL Save Changes]**」。

**在我的設定中找不到我的電子郵件給[!DNL Salesforce]**

如果您在[設定]底下沒有看到[我的電子郵件給[!DNL Salesforce]]，則可能是您的管理員未啟用它。 如果您的團隊剛接觸[!DNL Salesforce]，或您的團隊從未使用[!DNL Salesforce]提供的密件副本地址，就可能發生這種情況。

>[!NOTE]
>
>您需要管理員許可權才能設定此專案。

1. 按一下「**[!UICONTROL Setup]**」。
1. 按一下「**[!UICONTROL Email Administration]**」。
1. 按一下「**[!UICONTROL Email to Salesforce]**」。
1. 按一下「**[!UICONTROL Edit]**」。
1. 勾選「使用中」旁的方塊。
1. 按一下「**[!UICONTROL Save]**」。

## 將[!DNL Sales Insight Actions]個任務/提醒同步至[!DNL Salesforce]個任務 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在[!DNL Sales Insight Actions]中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-sync-settings-10.png)

1. 在「[!UICONTROL Admin Settings]」下（如果您不是管理員，則按「[!UICONTROL My Account]」），按一下「**[!UICONTROL Salesforce]**」。

   ![](assets/salesforce-sync-settings-11.png)

1. 按一下「**[!UICONTROL Sync Settings]**」標籤。

   ![](assets/salesforce-sync-settings-12.png)

1. 按一下「將Marketo銷售任務/提醒同步至[!DNL Salesforce]任務」旁的箭頭。

   ![](assets/salesforce-sync-settings-13.png)

1. 選擇所要的選項（預設會選取「不要同步至[!DNL Salesforce]個任務」）。

   ![](assets/salesforce-sync-settings-14.png)

## 第一次將[!DNL Sales Insight Actions]個任務與[!DNL Salesforce]同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

當您首次開啟[!DNL Sales Insight Actions]與[!DNL Salesforce]個任務之間的同步時，我們會匯入您的[!DNL Salesforce]個任務。 我們不會將您在[!DNL Sales Insight Actions]中擁有的任何目前任務推播到[!DNL Salesforce]。 若要減少雜訊和重複專案，唯一從[!DNL Sales Insight Actions]同步到[!DNL Salesforce]的任務是在您將[!DNL Sales Insight Actions]與SFDC同步之後建立的任務。

以下是當您同步[!DNL Sales Insight Actions]和SFDC任務時發生的情況：

當您在同步處理任務時按一下「儲存」，任務就會開始進行同步處理。 這最初需要一些時間。

任何在過去24小時內已更新或建立的提醒將會從SFDC提取至[!DNL Sales Insight Actions]。 同步是以到期日為基礎，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天到期的工作。

如果先前已開啟同步功能，而您又刪除了SFDC中的任何工作，則任何過去15天中刪除的工作都會從命令中心刪除。

只要同步處理已啟用，我們就會持續在[!DNL Sales Insight Actions]和SFDC之間同步處理工作。

初次同步之後，您在[!DNL Sales Insight Actions]中建立、編輯、完成或刪除的任何工作都會同步至[!DNL Salesforce]中的工作清單。 在[!DNL Salesforce]中建立、編輯、完成或刪除的任何專案都會在[!DNL Sales Insight Actions]中更新您的任務清單。

若要開啟此同步處理，只要在Web應用程式的[!UICONTROL Settings]頁面中勾選同步處理方塊即可。
