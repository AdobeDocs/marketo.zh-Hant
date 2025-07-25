---
unique-page-id: 10099077
description: 瞭解如何將種子清單匯入Marketo Engage執行個體。
title: 電子郵件傳遞能力套件 — 如何匯入種子清單
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Email Deliverability Power Pack：如何匯入種子清單 {#email-deliverability-power-pack-how-to-import-a-seed-list}

種子清單是多個信箱提供者(包括Google應用程式、Hotmail、Yahoo！等)的電子郵件帳戶清單，用於估計收件匣相對於垃圾郵件資料夾傳遞率。 以下是將該清單匯入Marketo Engage執行個體的步驟。

>[!IMPORTANT]
>
>本文適用於目前擁有使用中Everest訂閱的使用者。 如果您使用Inbox Tracker by Bird （先前稱為MessageBird），您可以在此找到教學課程[&#128279;](/help/marketo/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.md){target="_blank"}。

## 匯入種子清單 {#import-a-seed-list}

1. 在「我的Marketo」中，選取&#x200B;**[!UICONTROL Deliverability Tools]**。

   ![](assets/email-deliverability-power-pack-1.png)

1. 將會開啟[!DNL Everest]應用程式。 在左側導覽中，按一下&#x200B;**[!UICONTROL In-Flight]**&#x200B;並選取&#x200B;**[!UICONTROL Inbox Placement]**。

   ![](assets/email-deliverability-power-pack-2.png)

1. 按一下「**[!UICONTROL Manage Seed List]**」標籤。

   ![](assets/email-deliverability-power-pack-3.png)

1. 按一下&#x200B;**[!UICONTROL Actions]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Download: One Per Line]**。

   ![](assets/email-deliverability-power-pack-4.png)

   >[!NOTE]
   >
   >如果您希望[!DNL Everest]為您最佳化您的清單，請使用種子清單最佳化程式（在頁面頂端）。

1. 匯出後，清單會在瀏覽器的下載資料夾中顯示為.txt檔案。 擷取它，然後[將它匯入](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)您的Marketo執行個體作為靜態清單。

   ![](assets/email-deliverability-power-pack-5.png)

   >[!TIP]
   >
   >請務必將您的清單命名為容易找到的名稱。

   >[!CAUTION]
   >
   >您每月獲得的這些收件匣放置行銷活動數量有限。 若要檢視您獲得的數量，請檢視[!UICONTROL Subscription]中[!UICONTROL Account Settings] > [!UICONTROL Subscription]下的[!DNL Everest]區段。 若要取得更多資訊，請聯絡您的Marketo銷售代表。

## 取得新的種子清單 {#acquiring-new-seedlists}

您的種子清單可能每個月都會變更。 請務必定期登入Email Deliverability Power Pack，並檢查您的種子清單狀態。 新增地址或需要端點更新時，系統會透過應用程式左下角的通知圖示提醒您。

在Marketo中建立靜態清單後，您就可以開始傳送至該清單，以測試電子郵件的收件匣位置。
