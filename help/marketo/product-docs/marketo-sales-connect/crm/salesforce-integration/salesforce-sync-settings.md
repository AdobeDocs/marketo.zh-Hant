---
unique-page-id: 18317669
description: Salesforce同步設定 — Marketo檔案 — 產品檔案
title: Salesforce 同步設定
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 5%

---

# Salesforce 同步設定 {#salesforce-sync-settings}

## 透過API將電子郵件活動記錄到Salesforce {#logging-email-activity-to-salesforce-via-api}

若要使用此功能，您必須使用Salesforce的Enterprise/Unlimited版本，或是Professional版本（如果您已透過Web Services API購買整合）。

>[!PREREQUISITES]
>
>Salesforce與Sales Connect必須連線。

1. 在[!DNL Sales Connect]中，按一下右上方的齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-2.png)

1. 在[!UICONTROL My Account] ([!UICONTROL Admin Settings] （如果您是管理員）)底下，按一下&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-2.png)

1. 按一下「**[!UICONTROL Sync Settings]**」標籤。

   ![](assets/three-1.png)

1. 按一下[將電子郵件活動記錄到[!DNL Salesforce]]旁的箭頭。

   ![](assets/four-1.png)

1. 按一下「**[!UICONTROL Salesforce API]**」索引標籤。在此卡片中，您可以設定將資訊記錄到[!DNL Salesforce]的偏好設定。 完成時，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/five.png)

## 透過電子郵件將電子郵件活動記錄到Salesforce到Salesforce （密件副本） {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

啟用「傳送電子郵件至Salesforce （密件副本）」後，您將會收到銷售電子郵件的密件副本，且您的電子郵件會記錄為商機、潛在客戶和聯絡人的活動。

>[!PREREQUISITES]
>
>[!DNL Salesforce]與[!DNL Sales Connect]必須連線。

**透過電子郵件（密件副本）將您的電子郵件登入Salesforce**

1. 在[!UICONTROL Sales Connect]中，按一下右上方的齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-3.png)

1. 在[!UICONTROL My Account] ([!UICONTROL Admin Settings] （如果您是管理員）)底下，按一下&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-3.png)

1. 按一下「**[!UICONTROL Sync Settings]**」標籤。

   ![](assets/three-1.png)

1. 按一下「**[!UICONTROL Email to Salesforce (BCC)]**」標籤，然後按一下「**[!UICONTROL Activate]**」。

   ![](assets/six-2.png)

如果由於某種原因您的電子郵件至[!DNL Salesforce]位址沒有拉入，請依照下列步驟在您的[!DNL Salesforce]帳戶中啟動密件副本功能：

1. 登入您的[!DNL Salesforce]執行個體。
1. 在右上角找到您的使用者名稱，然後選取下拉式清單。
1. 選取「**[!UICONTROL My Settings]**」。
1. 選取「**[!UICONTROL Email]**」。
1. 選取「**[!UICONTROL My Email to Salesforce]**」。
1. 在此頁面中，您會看到標示為「傳送電子郵件至Salesforce位址」的欄位。 如果旁邊未填入任何內容，請向下捲動至「我的可接受電子郵件地址」。
1. 輸入您要密件副本的電子郵件地址。
1. 按一下「**[!UICONTROL Save Changes]**」。

**在我的設定中找不到我的電子郵件給[!DNL Salesforce]**

如果您在「設定」底下沒有看到「我的電子郵件至Salesforce」，表示您的管理員可能尚未啟用它。 如果您的團隊剛接觸[!DNL Salesforce]，或您的團隊從未使用[!DNL Salesforce]提供的密件副本地址，就可能發生這種情況。

>[!NOTE]
>
>您需要管理員許可權才能設定此專案。

1. 按一下「**[!UICONTROL Setup]**」。
1. 按一下「**[!UICONTROL Email Administration]**」。
1. 按一下「**[!UICONTROL Email to Salesforce]**」。
1. 按一下「**[!UICONTROL Edit]**」。
1. 勾選「[!UICONTROL Active]」旁的方塊。
1. 按一下「**[!UICONTROL Save]**」。

## 將Sales Connect工作/提醒同步至[!DNL Salesforce]個工作 {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. 按一下右上方的齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-3.png)

1. 在[!UICONTROL My Account] ([!UICONTROL Admin Settings] （如果您是管理員）)底下，按一下&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-2.png)

1. 按一下「**[!UICONTROL Sync Settings]**」標籤。

   ![](assets/three-1.png)

1. 按一下[!UICONTROL Sync Sales Engage Tasks/Reminders to Salesforce Tasks]旁的箭頭。

   ![](assets/seven-2.png)

1. 選擇所要的選項（預設會選取&quot;[!UICONTROL Do not sync to Salesforce tasks]&quot;）。

   ![](assets/eight.png)
