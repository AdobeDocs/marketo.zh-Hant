---
unique-page-id: 2950682
description: 建立方案通路-Marketo檔案——產品檔案
title: 建立方案渠道
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 建立程式通道{#create-a-program-channel}

方案是一項特定的行銷計畫。 該渠道的目的是提供機制，例如網路研討會、贊助或線上廣告。

>[!NOTE]
>
>**需要管理員權限**

>[!NOTE]
>
>進一步瞭解[programs](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)，這是Marketo最重要的元素。

1. 在&#x200B;**Admin**&#x200B;區段下，按一下&#x200B;**Tags**。

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >為什麼要標籤？ 頻道是描述程式的方式，就像其他標籤一樣。 這個頻道有特殊的額外功能。

1. 按一下&#x200B;**Channel**&#x200B;旁邊的&#x200B;**+**&#x200B;符號以展開並查看現有通道。

   ![](assets/image2014-9-24-12-3a58-3a33.png)

1. 在&#x200B;**New**&#x200B;下，按一下&#x200B;**New Channel**。

   ![](assets/image2014-9-24-12-3a58-3a53.png)

   >[!NOTE]
   >
   >**範例**
   >
   >渠道：廣告看板
   >
   >* 套用至：預設值
   >* 進展：會員，已參與（如果有疑問，這些工作正常）
   >* 成功：已參與

   >
   >渠道：政黨
   >
   >* 套用至：事件
   >* 進展：已邀請、已註冊、無展示及出席
   >* 成功：已參加

   >
   >查看現有渠道的「進度」，瞭解如何使用這些渠道。

1. 讓我們以黨的渠道為例。 為新&#x200B;**Channel**&#x200B;命名，然後選擇將應用該的程式類型。

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >申請什麼？ 程式有幾種類型。 將色版與正確的類型相符。 如果有疑問，請選擇&#x200B;**Default**。

   >[!NOTE]
   >
   >使用「包含網路研討會的活動」時，系統對應將會鎖定（視網路研討會整合的需要而定）且無法編輯。

   輸入前兩個程式的狀態名稱，然後按一下添加步驟。
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. 輸入另一個程式&#x200B;**Status**&#x200B;和&#x200B;**Step**&#x200B;編號，然後按一下&#x200B;**Add Step**。

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >**步驟**&#x200B;編號用於對程式狀態進行排序。 請記住，人們不能在這些進步步驟中倒退。 他們只能將狀態變更為較高或相等的值狀態。 當狀態要來回切換，而非進度時，請使用等值。

1. 輸入最後一個程式&#x200B;**Status**&#x200B;和&#x200B;**Step**&#x200B;編號。

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >使用「事件」類型時，系統需要對應「已註冊」、「候機清單」和「已出席」狀態。 因此，這些狀態無法隱藏。

1. 為&#x200B;**已註冊**&#x200B;選擇&#x200B;**移動簽入狀態**。

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. 為&#x200B;**Attended**&#x200B;選擇&#x200B;**Mobile Check-in Status**。

   ![](assets/image2014-9-24-15-3a40-3a21.png)

   >[!NOTE]
   >
   >**行動登入狀態**** **選項只有在頻道將用於事件程式時才可用。

   >[!NOTE]
   >
   >只有&#x200B;**已註冊**&#x200B;和&#x200B;**已註冊**&#x200B;的&#x200B;**行動登入狀態**&#x200B;的人員才會出現在[行動登入應用程式](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md)中。

   >[!TIP]
   >
   >如果在行動登入應用程式中建立新人員，則會在事件程式中設為「已註冊」。 如果某人已簽入應用程式上的事件，則會在事件程式中將其設為「已參加」。

1. 選擇&#x200B;**Success**&#x200B;程式狀態，然後按一下&#x200B;**Create**。

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   幹得漂亮！ 當您製作此類的新程式時，此新頻道將是您的選擇之一。
