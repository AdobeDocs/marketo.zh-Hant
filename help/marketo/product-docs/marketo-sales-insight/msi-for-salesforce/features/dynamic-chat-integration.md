---
description: Dynamic Chat整合 — Marketo檔案 — 產品檔案
title: Dynamic Chat整合
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 5%

---

# Dynamic Chat整合 {#dynamic-chat-integration}

進一步瞭解Dynamic Chat與Sales Insight的整合。

>[!PREREQUISITES]
>
>* 您的Sales Insight SFDC套件必須是版本 [1.9或更新版本](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* 您必須擁有 [Dynamic Chat整合](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} 設定

## Marketo Sales Insight設定索引標籤 {#marketo-sales-insight-configuration-tab}

請依照下列步驟來啟用Dynamic Chat整合。

1. 登入您的Salesforce帳戶，按一下標籤列結尾的+ ，然後按一下 **Marketo銷售分析設定**.

1. 按一下以展開「Visualforce面板」。

   ![](assets/dynamic-chat-integration-1.png)

1. 選取 **啟用Dynamic Chat資料** 核取方塊。

   ![](assets/dynamic-chat-integration-2.png)

## 功能概述 {#feature-overview}

Sales Insight使用者可以利用以下Dynamic Chat活動……

參與對話方塊：登入Marketo，並在訪客點按聊天機器人參與對話方塊時填入Sales Insight。

* 對話名稱
* 頁面 URL
* 狀態（已啟動/已捨棄/已完成）

已排程約會：登入Marketo，並在訪客透過聊天機器人成功排程約會時填入銷售分析。

* 對話名稱
* 專員
* 頁面 URL
* 排程日期（插入日期和時間戳記）
* 狀態（已排程、已重新排程、已取消）

已達成目標：當訪客達成任何對話方塊流程中的目標時，登入Marketo並填入銷售分析中。

* 對話名稱
* 目標名稱
* 頁面 URL

與檔案互動：訪客與透過聊天機器人共用的檔案互動時，登入Marketo並填入銷售分析中。

* 對話名稱
* 文件
* 狀態

可在見解儀表板中使用聊天活動。

![](assets/dynamic-chat-integration-3.png)

潛在客戶面板和聯絡人面板中提供「聊天」標籤。 其中包括「活動型別」、「對話方塊名稱」和「日期」欄。

![](assets/dynamic-chat-integration-4.png)

您可以按一下活動型別，以瞭解更多有關活動型別的資訊。

![](assets/dynamic-chat-integration-5.png)

同樣地，「帳戶」和「商機」面板包括「名稱」、「活動型別」、「對話方塊名稱」和「日期」欄。

![](assets/dynamic-chat-integration-6.png)

Chat標籤也包含在您的全域Marketo標籤中。 它包含三種活動型別（參與對話方塊、排程約會、達成目標），以及下列欄：

* 個人
* 帳戶
* 活動型別（參與對話方塊、排程約會、達成目標）
* 對話名稱
* 日期與時間戳記

同樣地，您可以按一下某個活動型別以深入瞭解該活動型別。

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>如果「啟用Dynamic Chat資料」核取方塊已停用，則下列功能將會停用：
>
>* 前瞻分析儀表板（智慧格線和每週清單檢視）中包含聊天活動的列
>* Lead、Contact、Account和Opportunity面板中的Chat標籤
>* 「全域Marketo」標籤中的「聊天」標籤
>
>不能只停用其中一項功能。

