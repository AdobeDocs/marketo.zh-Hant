---
description: Dynamic Chat概述 — Marketo檔案 — 產品檔案
title: 動態聊天概述
hide: true
hidefromtoc: true
source-git-commit: 121b2f1dd3bc807feaf8e8682307074bac43e12e
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# 動態聊天概述 {#dynamic-chat-overview}

動態聊天功能可讓您利用簡單易用的介面，將目標同時鎖定在造訪您網站的人員和帳戶。 收集相關內容，例如姓名、聯繫資訊和自由文本。 網站訪客也可以預訂與您的銷售團隊的會議。 動態聊天活動和參與資料可用來新增成員至Marketo方案並觸發跨通道活動。

>[!NOTE]
>
>Dynamic Chat正在逐步推出，目前可用性有限。 本頁將隨正式發行(GA)詳細資訊的提供而更新。

## 整合 {#integrations}

Dynamic Chat的一個關鍵元件是其與Marketo訂閱原生介面的功能。 若要充分運用這項整合的完整功能，您必須先啟動資料同步。 視您的Marketo資料庫大小而定，初始資料可能需要24小時， [一次性同步](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) 完成。

已同步下列項目：

* 人員欄位資料
* 公司欄位資料
* 活動資料

## 對話方塊 {#dialogues}

對話方塊代表單一聊天參與。 您可以將其想像成容器，內含您與網站訪客進行有趣的聊天對話所需的所有內容。 在每個對話框中，可以指定希望對話框顯示在哪個頁面上、希望向誰顯示對話框，以及對話框本身的內容和流。 此外，您還可以找到量度，以了解對話方塊的執行成效。 [深入了解對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## 設定 {#configuration}

在「配置」頁簽中，自定義各種對話框的外觀和風格。 變更字型、顏色、回應時間等！ [進一步了解配置](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## 日曆 {#calendar}

在「日曆」標籤中，連接您的（Outlook或Gmail）日曆，以用於查特機器人的約會排程。 當用戶的日曆連接到動態聊天后，該用戶將被添加到隊列中，其日曆將可供網站訪客安排約會。

您也可以自訂在訪客在使用者日曆上排程約會時，傳送給訪客的邀請內文。

## 會議 {#meetings}

這是網站訪客透過各種對話方塊排程的所有約會。 在此，您將找到預訂約會的人員的電子郵件地址、預訂約會的座席、安排約會的時間以及會議是否已發生。

## 路由 {#routing}

您可以在此處查看已連接其日曆的所有座席的清單，以及向網站訪客顯示這些座席的順序。 會議按循規蹈矩，因此，如果你有五名代理和三號探員參加了最後一次會議，四號探員會得到下一次會議，然後五號探員會回到一號探員。

## 常見問題集 {#faq}

**動態聊天是否允許即時聊天？**

不會，它只會使用預先決定的回應。

**如何鎖定匿名人員？**

在對話方塊中，您需要使用 _人員電子郵件為空_ 屬性。

**您是否支援AI/NLP功能？**

我們不支援AI/NLP功能。

**資料儲存多久以用於報告？**

90天。

**Dynamic Chat除了英文以外還提供任何語言嗎？**

現在不行。
