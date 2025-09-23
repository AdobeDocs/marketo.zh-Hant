---
description: Dynamic Chat整合 — Marketo檔案 — 產品檔案
title: Dynamic Chat 整合
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 7%

---

# Dynamic Chat 整合 {#dynamic-chat-integration}

深入瞭解Dynamic Chat與銷售Insight的整合。

>[!PREREQUISITES]
>
>* 您的銷售Insight SFDC套件必須是[2.4.0或更新版本](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* 您必須設定[Dynamic Chat整合](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* 確定在您的Sales Insight [作業設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"}中，已填入「API秘密金鑰」欄位。 如果您沒有，請在[這裡](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}瞭解如何擷取它。

## [!DNL Marketo Sales Insight]設定標籤 {#marketo-sales-insight-configuration-tab}

請依照下列步驟來啟用[!DNL Dynamic Chat]整合。

1. 登入您的[!DNL Salesforce]帳戶，按一下標籤列結尾的+並按一下&#x200B;**[!DNL Marketo Sales Insight Config]**。

1. 按一下以展開「[!UICONTROL Visualforce Panel]」。

   ![](assets/dynamic-chat-integration-1.png)

1. 選取&#x200B;**[!UICONTROL Enable Dynamic Chat Data]**&#x200B;核取方塊。

   ![](assets/dynamic-chat-integration-2.png)

## 功能概觀 {#feature-overview}

[!DNL Dynamic Chat]個使用者可以利用下列[!DNL Sales Insight]個活動……

參與對話方塊：登入Marketo並在訪客點按聊天機器人並參與對話方塊時填入[!DNL Sales Insight]。

* 對話名稱
* 頁面 URL
* 狀態（已啟動/已捨棄/已完成）

已排程約會：登入Marketo並在訪客透過聊天機器人成功排程約會時填入[!DNL Sales Insight]。

* 對話名稱
* 專員
* 頁面 URL
* 排程日期（插入日期和時間戳記）
* 狀態（已排程、已重新排程、已取消）

已達成目標：訪客在任何對話方塊流程中達成目標時登入Marketo並填入[!DNL Sales Insight]。

* 對話名稱
* 目標名稱
* 頁面 URL

與檔案互動：訪客與透過聊天機器人共用的檔案互動時登入Marketo並填入[!DNL Sales Insight]。

* 對話名稱
* 文件
* 狀態

可在見解儀表板中使用聊天活動。

![](assets/dynamic-chat-integration-3.png)

潛在客戶面板和聯絡人面板中提供「聊天」標籤。 它包含[!UICONTROL Activity Type]、[!UICONTROL Dialogue Name]和[!UICONTROL Date]欄。

![](assets/dynamic-chat-integration-4.png)

您可以按一下活動型別，以瞭解更多有關活動型別的資訊。

![](assets/dynamic-chat-integration-5.png)

同樣地，「帳戶」和「商機」面板包含[!UICONTROL Name]、[!UICONTROL Activity Type]、[!UICONTROL Dialogue Name]和[!UICONTROL Date]欄。

![](assets/dynamic-chat-integration-6.png)

Chat標籤也包含在您的全域Marketo標籤中。 它包含三種活動型別([!UICONTROL Engaged Dialogue]、[!UICONTROL Scheduled Appointment]、[!UICONTROL Reached Goal])，以及下列資料行：

* [!UICONTROL Person]
* [!UICONTROL Account]
* [!UICONTROL Activity type] ([!UICONTROL Engaged Dialogue]， [!UICONTROL Scheduled Appointment]， [!UICONTROL Reached Goal])
* [!UICONTROL Dialogue Name]
* [!UICONTROL Date]

同樣地，您可以按一下某個活動型別以深入瞭解該活動型別。

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>如果&quot;[!UICONTROL Enable Dynamic Chat data]&quot;核取方塊已停用，則會停用下列功能：
>
>* 前瞻分析儀表板（智慧格線和每週清單檢視）中包含聊天活動的列
>* Lead、Contact、Account和Opportunity面板中的Chat標籤
>* 「全域Marketo」標籤中的「聊天」標籤
>
>不能只停用其中一項功能。
