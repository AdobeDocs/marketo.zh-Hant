---
unique-page-id: 7514898
description: 瞭解如何使用「已要求Campaign」為銷售設定觸發Smart Campaign。 讓銷售人員從CRM要求銷售機會的行銷活動。
title: 使用「已請求行銷活動」設定銷售的觸發程序智慧行銷活動
exl-id: ed6d7c27-d54b-48e3-af67-19503da4ef56
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 11%

---

# 使用「已請求行銷活動」設定銷售的觸發程序智慧行銷活動 {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

Marketo最酷的功能之一，是讓銷售人員參與行銷工作。 他們在前線，與人互動。 銷售代表應該有能力將行銷導向正確的方向。

>[!NOTE]
>
>要要求的Smart Campaign範例：
>
>1. **長期Nurture** — 當他們今年沒有預算，而您想要留心時
>1. **有效的銷售週期** — 當銷售人員除了他們自己的訊息之外，不想給該人員任何訊息時。 （使用行銷活動暫停旗標來暫時取消訂閱）
>
>詢問銷售團隊他們想要自動化和設定什麼。

1. 建立智慧型行銷活動。

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-1.png)

1. 找到「**[!UICONTROL Campaign is Requested]**」觸發程序，將其拖曳至版面。

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-2.png)

1. 來源選擇指出將接受哪種請求。 如需Salesforce功能，請選擇&#x200B;**[!UICONTROL Sales Insight]**。

   >[!TIP]
   >
   >來源運運算元用於保全性。 您可以將行銷活動限製為僅由特定來源提出的請求，例如其他Smart Campaigns或開發人員。 如果要允許來自所有來源的請求，請在第一個方塊中選擇&#x200B;**[!UICONTROL Is Any]**。
   >
   >_記住_，選擇Sales Insight後，它就會神奇地顯示在銷售方塊中。 避免新增太多，否則會遭到忽略。

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-3.png)

這是將行銷範圍延伸至其他部門的絕佳方式。 設定各種要自動化的行銷活動。

>[!TIP]
>
>清楚地命名您的Smart Campaign。 它們會以您指定的方式顯示在銷售Insight中。
