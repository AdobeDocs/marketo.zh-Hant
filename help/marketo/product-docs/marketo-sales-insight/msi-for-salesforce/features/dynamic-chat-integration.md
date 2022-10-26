---
description: Dynamic Chat整合 — Marketo檔案 — 產品檔案
title: 動態聊天整合
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: 9d5c941dc4869b03787a6135550a133ce12b365b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 3%

---

# 動態聊天整合 {#dynamic-chat-integration}

進一步了解與Sales Insight的Dynamic Chat整合。

>[!PREREQUISITES]
>
>* 您的Sales Insight SFDC包必須是版本 [1.9或更高版本](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* 您必須擁有 [動態聊天整合](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;}已設定


## Marketo Sales Insight設定標籤 {#marketo-sales-insight-configuration-tab}

請依照下列步驟啟用動態聊天整合。

1. 登入您的Salesforce帳戶，按一下標籤列結尾的+，然後按一下 **Marketo Sales Insight設定**.

1. 按一下以展開「視覺效果面板」。

   ![](assets/dynamic-chat-integration-1.png)

1. 選取 **啟用動態聊天資料** 核取方塊。

   ![](assets/dynamic-chat-integration-2.png)

## 功能概述 {#feature-overview}

Sales Insight使用者可運用下列動態聊天活動……

參與對話：登入Marketo，並在訪客點按動作機器人並參與對話時填入Sales Insight。

* 對話名稱
* 頁面URL
* 狀態（已啟動/已丟棄/已完成）

計畫約會：當訪客透過動作機器人成功排程約會時，登入Marketo並填入Sales Insight。

* 對話名稱
* 代理
* 頁面URL
* 排程於（插入日期和時間戳記）
* 狀態（已計畫、已重新計畫、已取消）

已達目標：登入Marketo，當訪客在任何對話方塊流程中達到目標時，便填入Sales Insight。

* 對話名稱
* 目標名稱
* 頁面URL

與檔案互動：登入Marketo，並在訪客與透過聊天機器人共用的檔案互動時填入Sales Insight。

* 對話名稱
* 文件
* 狀態

可在「前瞻分析控制面板」中使用聊天活動。

![](assets/dynamic-chat-integration-3.png)

「銷售機會」和「聯繫人」面板中有「聊天」頁簽。 其中包含「活動類型」、「對話方塊名稱」和「日期」欄。

![](assets/dynamic-chat-integration-4.png)

您可以按一下活動類型，以深入了解。

![](assets/dynamic-chat-integration-5.png)

同樣，「帳戶」和「機會」面板包括「名稱」、「活動類型」、「對話名稱」和「日期」列。

![](assets/dynamic-chat-integration-6.png)

您的「全域Marketo」標籤也包含「聊天」標籤。 它包括三種活動類型（參與對話、排程約會、達成目標），以及下列欄：

* 個人
* 帳戶
* 活動類型（參與對話、已排程約會、已達目標）
* 對話名稱
* 日期和時間戳記

您也可以按一下活動類型，以進一步了解。

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>如果「啟用動態聊天資料」核取方塊已停用，則會停用下列功能：
>
>* 在Insights Dashboard中與聊天活動列（智慧格線和每週清單檢視）
>* 「銷售機會」、「聯繫人」、「帳戶」和「銷售機會」面板中的「聊天」頁簽
>* 「全域Marketo」標籤中的「聊天」標籤
>
>不能僅禁用其中一項功能。

