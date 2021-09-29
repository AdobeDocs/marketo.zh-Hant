---
description: Dynamic Chat概述 — Marketo檔案 — 產品檔案
title: 動態聊天概述
hide: true
hidefromtoc: true
source-git-commit: afc7c8352b4470bfc367f3d16836fb14d55b8821
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# 動態聊天概述 {#dynamic-chat-overview}

動態聊天允許您利用易於使用的介面來定位兩個銷售機會(PEOPLE?) 和他們（拜訪您的？）的帳戶 網站。 收集相關內容，例如其名稱、聯繫資訊和自由文本。 網站訪客也可以預訂與您的銷售團隊的會議。 動態聊天活動和參與資料可用來新增成員至Marketo方案並觸發跨通道活動。

>[!NOTE]
>
>動態聊天正在逐步推出，所有訂閱都將在2022年春季前擁有存取權。 如需詳細資訊，請連絡您的客戶成功經理。

## 整合 {#integrations}

Dynamic Chat的一個關鍵元件是其與Marketo訂閱原生介面的功能。 若要充分運用這項整合的完整功能，您必須先啟動資料同步。 根據Marketo資料庫的大小，初始資料[一次同步](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md)最多可能需要24小時才能完成。 平均同步時間不到2小時。

已同步下列項目：

* 潛在客戶欄位資料
* 公司欄位資料
* 活動資料

## 對話方塊 {#dialogues}

對話方塊代表單一聊天參與。 您可以將其想像成容器，內含您與網站訪客進行有趣的聊天對話所需的所有內容。 在每個對話框中，可以指定希望對話框顯示在哪個頁面上、希望向誰顯示對話框，以及對話框本身的內容和流。 此外，您還可以找到量度，以了解對話方塊的執行成效。 [深入了解對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)。

## 設定 {#configuration}

在「配置」頁簽中，自定義各種對話框的外觀和風格。 變更字型、顏色、回應時間等！ [深入了解設定](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md)。

## 日曆 {#calendar}

在「日曆」標籤中，連接您的（Outlook或Gmail）日曆，以用於查特機器人的約會排程。 當用戶的日曆連接到動態聊天后，該用戶將被添加到隊列中，其日曆將可供網站訪客安排約會。

您也可以自訂邀請電子郵件的內文？ 當訪客在使用者日曆上排程約會時，就會傳送給訪客。

## 會議 {#meetings}

這是網站訪客透過各種對話方塊排程的所有約會。 在此，您將找到預訂約會的主管的電子郵件地址、他們與哪個座席預訂約會、計畫約會的時間以及會議是否已發生。

## 路由 {#routing}

在這裡，您可以看到所有已連接其日曆的座席的清單，以及將向網站訪客顯示的順序。會議會按循序方式進行，因此，如果您有五個座席和三個座席參加了最後一次會議，則四座座席將得到下一個，然後是五座，然後返回一座座席。

## 常見問題集 {#faq}

**動態聊天是否允許即時聊天？**

不會，它只會使用預先決定的回應。

**如何鎖定匿名的線索？**

在對話方塊中，您需要使用&#x200B;_Lead Email is Empty_&#x200B;屬性。

**您是否支援AI/NLP功能？**

我們不支援AI/NLP功能。

**資料儲存多久以用於報告？**

90天。

**Dynamic Chat除了英文以外還提供任何語言嗎？**

現在不行。
