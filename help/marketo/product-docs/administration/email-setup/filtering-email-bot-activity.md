---
description: 篩選電子郵件Bot活動 — Marketo文檔 — 產品文檔
title: 篩選電子郵件Bot活動
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 524e185e255503ac44bb73303091a59b2d60242a
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# 篩選電子郵件Bot活動 {#filtering-email-bot-activity}

有時，電子郵件僵屍活動會錯誤地開啟電子郵件並按一下資料。 按照以下步驟修復此問題。

我們使用三種不同的方法來確認bot活動：

* 匹配 [互動式廣告局bot清單](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;:與IAB UA/IP（用戶代理/IP地址）清單中的任何內容相匹配的活動將標籤為bot。
* 與鄰近模式匹配：當同時發生兩個以上的活動時（不到兩秒），它們被標識為bot。

根據電子郵件連結按一下和電子郵件開啟活動，新屬性將填充以下值：

* 被標識為bot的活動將「Bot Activity」（Bot活動）作為「True」，「Bot Activity Pattern」（Bot活動模式）作為已標識的模式/方法
* 被標識為非bot的活動將「Bot Activity」（Bot活動）設定為「False」（假），「Bot Activity Pattern」（Bot活動模式）設定為「N/A」(N/A)
* 在引入這些屬性之前發生的活動將「Bot Activity」(Bot Activity)作為「 」（空），「Bot Activity Pattern 」(Bot Activity Pattern)作為「 」（空）)

1. 按一下 **管理**。

   ![](assets/filtering-email-bot-activity-1.png)

1. 按一下 **電子郵件**。

   ![](assets/filtering-email-bot-activity-2.png)

1. 按一下 **Bot活動** 頁籤。

   ![](assets/filtering-email-bot-activity-3.png)

1. 選擇 **與IAB清單匹配**。 **與鄰近陣列匹配**，或兩者兼有。

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>您可以選擇對bot活動進行篩選 **或** 已記錄。 如果選擇篩選，則可能會看到電子郵件中的一個刪除，並在清除假活動時按一下

**可選步驟**:要禁用此功能，只需取消選擇滑塊。 如果禁用，則資料不會重置。

>[!TIP]
>
>通過「Clicked Link in E-mail」和「Open E-mail」過濾器中的「Is Bot Activity」布爾值（是/否）和「Bot Activity Pattern」，以及「Clicks Link in E-mail」和「Open E-mail」觸發器，利用智慧清單中的bot活動資料。
