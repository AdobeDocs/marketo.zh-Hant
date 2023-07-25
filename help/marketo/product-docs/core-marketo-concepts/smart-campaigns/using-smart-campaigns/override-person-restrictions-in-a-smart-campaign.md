---
unique-page-id: 1147066
description: 覆寫Smart Campaign中的人員限制 — Marketo檔案 — 產品檔案
title: 覆寫智慧行銷活動中的人員限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# 覆寫智慧行銷活動中的人員限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo可讓您設定符合智慧行銷活動資格的人數上限；這可協助您避免意外傳送電子郵件給整個資料庫。 如果您想要 _覆寫_ 此限制如下。

>[!PREREQUISITES]
>
>請確定 [為智慧行銷活動啟用人員限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) 在Marketo Admin中。

1. 在行銷活動中，前往您的智慧行銷活動並按一下 **排程**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. 在Smart Campaign設定中，按一下 **編輯**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >預設限製為「管理員」中設定的限制。

1. 輸入新限制，然後按一下 **儲存。**

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   如果符合資格的人數超過設定的限制，則智慧型行銷活動不會執行。

   >[!CAUTION]
   >
   >使用此功能時請務必小心，以免不小心納入太多人員。
