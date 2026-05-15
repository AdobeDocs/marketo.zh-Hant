---
unique-page-id: 2360217
description: 如何在Revenue Cycle Analytics中設定首次接觸和多點接觸歸因、潛在客戶轉換，以及受行銷影響的機會選項。
title: 變更分析的歸因設定
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 160
ht-degree: 9%

---

# 變更分析的歸因設定 {#change-attribution-settings-for-analytics}

您可以變更Marketo將聯絡人與首次接觸與多次接觸歸因的機會、潛在客戶轉換量度及行銷影響的機會標幟連結的方式。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 按一下「**[!UICONTROL Revenue Cycle Analytics]**」。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 按一下&#x200B;**[!UICONTROL Attribution]**&#x200B;下的&#x200B;**[!UICONTROL Edit]**&#x200B;連結。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >變更此設定不會修改任何Marketo資料；而是會變更報表的執行方式。 這可以隨時還原。

1. 選取選項並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL Explicit]**：只有具有角色的連絡人（預設）。
   >
   >**[!UICONTROL Hybrid]**：具有角色的連絡人（如果有的話）。 如果沒有可用專案，則會使用帳戶中的所有連絡人。
   >
   >**[!UICONTROL Implicit]**：所有連絡人，不論角色為何。

>[!CAUTION]
>
>使用&#x200B;**[!UICONTROL Implicit]**&#x200B;時，無論角色為何，Marketo一律會檢查與帳戶相關聯的所有連絡人。 **Marketo強烈建議使用[!UICONTROL Explicit]模式**。 使用[!UICONTROL Implicit]可能會產生誤判；也就是說，雖然對商機沒有實際影響，但擁有商機評分的人員。 請謹慎使用[!UICONTROL Implicit]。
