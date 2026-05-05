---
unique-page-id: 2360243
description: 設定符合Smart Campaign資格的人數上限，以避免意外傳送電子郵件給整個資料庫。
title: 啟用智慧行銷活動人員限制
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
source-git-commit: df76402e5fb0c002afeb04d41c52801be67a7136
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 14%

---

# 啟用智慧行銷活動人員限制 {#enable-person-restrictions-for-smart-campaigns}

Marketo提供的一項功能，可限制符合Smart Campaign資格的&#x200B;_上限_&#x200B;人數。 這樣可避免不小心將整個資料庫傳送至電子郵件。

>[!NOTE]
>
>**需要管理員權限**

>[!CAUTION]
>
>這僅適用於批次行銷活動和電子郵件方案。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/enable-person-restrictions-for-smart-campaigns-1.png)

1. 按一下「**[!UICONTROL Smart Campaign]**」。

   ![](assets/enable-person-restrictions-for-smart-campaigns-2.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/enable-person-restrictions-for-smart-campaigns-3.png)

   >[!CAUTION]
   >
   >如果符合執行Smart Campaign的資格人數超過所設定的限制，則完全不會執行。

1. 輸入限制並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/enable-person-restrictions-for-smart-campaigns-4.png)

   >[!TIP]
   >
   >將此欄位設為空白以停用此功能。

   >[!CAUTION]
   >
   >此限制會套用至所有Smart Campaigns，但可在行銷活動層級覆寫。 瞭解如何在Smart Campaign[&#128279;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)中覆寫人員限制。

>[!MORELIKETHIS]
>
>[在智慧行銷活動中覆寫人員限制](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
