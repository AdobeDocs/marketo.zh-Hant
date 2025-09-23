---
description: 回覆記錄 — Marketo檔案 — 產品檔案
title: 回應記錄
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 2%

---

# 回應記錄 {#reply-logging}

「銷售Insight動作」可讓您自動將潛在客戶的回覆記錄到[!DNL Salesforce]。 允許您執行此動作的結構是根據我們的電子郵件回覆追蹤。 如果我們可以追蹤潛在客戶的回覆，就可以將該回覆記錄到[!DNL Salesforce]。

## 需求 {#requirements}

* 必須透過API記錄來記錄電子郵件
* 必須能夠[追蹤回覆](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
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
1. 在[!UICONTROL Task Type Picklist Values]底下，按一下&#x200B;**[!UICONTROL New]**。
1. 在空白方塊中輸入「Reply」。 請確定您將&#39;R&#39;變成大寫，然後按一下&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >您不需要在「型別」選擇清單下選取「預設」。 [!DNL Sales Insight Actions]將看到此Activity Type可在您的[!DNL Salesforce]執行個體中使用，並相應地填入傳入活動上的工作列位。
