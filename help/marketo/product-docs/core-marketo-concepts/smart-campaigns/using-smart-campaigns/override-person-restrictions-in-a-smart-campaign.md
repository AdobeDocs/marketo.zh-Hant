---
unique-page-id: 1147066
description: 在Smart Campaign中覆寫人員限制 — Marketo檔案 — 產品檔案
title: 覆寫智慧行銷活動中的人員限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# 覆寫智慧行銷活動中的人員限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage可讓您設定符合Smart Campaign資格的人數上限；這可協助您避免意外傳送電子郵件給整個資料庫。 若您要&#x200B;_覆寫_&#x200B;此限制，請依下列方法操作。

>[!PREREQUISITES]
>
>請務必在Marketo管理員中[啟用智慧行銷活動的人員限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"}。

1. 在&#x200B;**[!UICONTROL 行銷活動]**&#x200B;中，移至您的Smart Campaign並按一下&#x200B;**[!UICONTROL 排程]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. 在Smart Campaign設定中，按一下&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >預設限製為「管理員」中設定的限制。

1. 輸入新的限制，然後按一下[儲存]。**&#x200B;**

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   如果符合資格的人數超過設定的限制，Smart Campaign將不會執行。

   >[!CAUTION]
   >
   >使用此功能時請小心，以免意外包含太多人員。
