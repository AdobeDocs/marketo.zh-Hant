---
unique-page-id: 14352480
description: 回覆記錄(SFDC) - Marketo檔案 — 產品檔案
title: 回覆記錄(SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 回覆記錄(SFDC) {#reply-logging-sfdc}

Sales Connect可協助您自動將潛在客戶的回覆記錄到Salesforce。 允許您執行此動作的結構是根據我們的電子郵件回覆追蹤。 如果我們可以追蹤潛在客戶的回覆，我們就能將該回覆記錄到Salesforce。

## 需求 {#requirements}

* 必須透過API記錄來記錄電子郵件
* 必須能夠[追蹤回覆](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* 必須與[!DNL Salesforce]連線
* 必須有[!DNL Salesforce]個[API呼叫](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)可用

## 啟用回覆記錄 {#enable-reply-logging}

1. 若要啟用回覆記錄，您可以前往[!DNL Salesforce]設定頁面。 核取API記錄後，您將會看到核取&#x200B;_記錄回覆_&#x200B;的選項。

   >[!NOTE]
   >
   >回覆記錄會遵循您針對記錄已傳送電子郵件所制定的相同規則。 這包括如何記錄電子郵件；至銷售機會和聯絡人；當有重複記錄時；如果找不到相符的記錄。

## 設定在[!DNL Salesforce]中回覆的型別 {#setting-type-to-reply-in-salesforce}

從您的[!DNL Salesforce]報表取得有意義的資料很重要。 讓型別欄位填入為「回覆」的功能可讓您透過報表取得該資料。 與您的`[!DNL Salesforce] admin`合作以取得此設定。

1. 前往「**[!UICONTROL Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Activities]** > **[!UICONTROL Task Fields]**」。
1. 按一下「**[!UICONTROL Type]**」。
1. 在任務型別選擇清單值下，按一下&#x200B;**[!UICONTROL New]**。
1. 在空白方塊中輸入「Reply」。 請確定您將&#39;R&#39;變成大寫，然後按一下&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >您不需要在「型別」選擇清單下選取「預設」。 [!DNL Sales Connect]將看到此Activity Type可在您的[!DNL Salesforce]執行個體中使用，並相應地填入傳入活動上的工作列位。
