---
description: 篩選電子郵件Bot活動 — Marketo文檔 — 產品文檔
title: 篩選電子郵件Bot活動
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 篩選電子郵件Bot活動 {#filtering-email-bot-activity}

有時，電子郵件僵屍活動會錯誤地開啟電子郵件並按一下資料。 這是如何解決的。

>[!NOTE]
>
>使用 [IAB/ABC國際蜘蛛和機器人清單](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/)，所有與清單中任何內容匹配的IP或用戶代理開啟/按一下活動都將被標識為bot活動，並且不會登錄Marketo。

1. 按一下 **管理**。

   ![](assets/filtering-email-bot-activity-1.png)

1. 按一下 **電子郵件**。

   ![](assets/filtering-email-bot-activity-2.png)

1. 按一下 **Bot活動** 頁籤。

   ![](assets/filtering-email-bot-activity-3.png)

1. 按一下滑塊以啟用 **篩選Bot活動**。

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>您可以單獨選擇是否記錄bot活動。 如果您選擇不這樣做，您可能會看到電子郵件中的一滴資訊開啟，並在過濾掉假號時按一下。

**可選步驟**:要禁用該功能，只需取消選擇滑塊。 如果禁用，則「過去90天的Bot活動」資料會 **不** 重置。

>[!TIP]
>
>通過「Is Bot Activity」布爾值(yes/no)或適用的篩選器/觸發器約束，利用智慧清單中的bot活動資料。
