---
unique-page-id: 1147066
description: 瞭解如何在Smart Campaign中覆寫人員限制。 即使人員達到通訊限制，仍可執行。
title: 覆寫智慧行銷活動中的人員限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 141
ht-degree: 9%

---

# 覆寫智慧行銷活動中的人員限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage可讓您設定符合Smart Campaign資格的人數上限；這可協助您避免意外傳送電子郵件給整個資料庫。 若您要&#x200B;_覆寫_&#x200B;此限制，請依下列方法操作。

>[!PREREQUISITES]
>
>請務必在Marketo管理員中[啟用智慧行銷活動的人員限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"}。

1. 在&#x200B;**[!UICONTROL Marketing Activities]**&#x200B;中，前往您的Smart Campaign並按一下&#x200B;**[!UICONTROL Schedule]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. 在Smart Campaign設定中，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >預設限製為「管理員」中設定的限制。

1. 輸入新的限制，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   如果符合資格的人數超過設定的限制，Smart Campaign將不會執行。

   >[!CAUTION]
   >
   >使用此功能時請小心，以免意外包含太多人員。
