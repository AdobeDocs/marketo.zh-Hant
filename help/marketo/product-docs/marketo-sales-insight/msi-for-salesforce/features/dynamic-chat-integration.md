---
description: 動態聊天整合 — Marketo文檔 — 產品文檔
title: 動態聊天整合
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: 676bd1c43fc62b2eae0e4536fb738b5be863e196
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 3%

---

# 動態聊天整合 {#dynamic-chat-integration}

瞭解有關與Sales Insight的動態聊天整合的詳細資訊。

>[!PREREQUISITES]
>
>* 您的Sales Insight SFDC包必須是版本 [1.9或更高版本](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;
>
>* 您必須 [動態聊天整合](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md)已設定{target=&quot;_blank&quot;


## MarketoSales Insight配置頁籤 {#marketo-sales-insight-configuration-tab}

按照以下步驟啟用動態聊天整合。

1. 登錄到Salesforce帳戶，按一下頁籤欄末尾的+，然後按一下 **MarketoSales Insight配置**。

1. 按一下以展開「Visualforce Panel（VisualForce面板）」。

   ![](assets/dynamic-chat-integration-1.png)

1. 選擇 **啟用動態聊天資料** 複選框。

   ![](assets/dynamic-chat-integration-2.png)

## 功能概述 {#feature-overview}

Sales Insight用戶可以利用以下動態聊天活動……

已參與對話：當訪問者按一下聊天機並參與對話框時，登錄Marketo並填充到Sales Insight中。

* 對話名稱
* 頁面URL
* 狀態（已啟動/已丟棄/已完成）

計畫約會：當訪問者通過聊天機成功安排約會時，登錄Marketo並填充到Sales Insight中。

* 對話名稱
* 代理
* 頁面URL
* 計畫時間（插入日期和時間戳）
* 狀態（已計畫、已重新計畫、已取消）

已達目標：當訪問者在任何對話框流中達到目標時，登錄Marketo並填充到Sales Insight中。

* 對話名稱
* 目標名稱
* 頁面URL

Lead和Contact面板中有「聊天」頁籤。 它包括「活動類型」、「對話框名稱」和「日期」列。

![](assets/dynamic-chat-integration-3.png)

通過按一下活動類型，您可以瞭解有關該活動類型的詳細資訊。

![](assets/dynamic-chat-integration-4.png)

同樣，「帳戶」和「業務機會」面板包括「名稱」、「活動類型」、「對話框名稱」和「日期」列。

![](assets/dynamic-chat-integration-5.png)

「聊天」頁籤還包含在「全局Marketo」頁籤中。 它包括三種活動類型（「已參與」對話框、「計畫約會」、「已達目標」），以及以下列：

* 個人
* 帳戶
* 活動類型（參與對話框、計畫約會、已達目標）
* 對話名稱
* 日期和時間戳

同樣，您可以通過按一下某個活動類型來瞭解有關該活動類型的詳細資訊。

![](assets/dynamic-chat-integration-6.png)

>[!NOTE]
>
>MSI中將在即將發佈的版本中提供「與文檔交互」活動。
