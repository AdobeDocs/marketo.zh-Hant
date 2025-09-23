---
unique-page-id: 37355758
description: 將成員新增至事件程式 — Marketo檔案 — 產品檔案
title: 新增成員至事件方案
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 9%

---

# 新增成員至事件方案 {#adding-members-to-an-event-program}

本文僅適用於使用事件上限或事件目標的使用者。

>[!CAUTION]
>
>將人員清單直接匯入事件方案，將會防止這些記錄被計算在「目標追蹤」報表和「事件上限進展」報表的實際註冊中。 請依照下列指示操作，確保計算您的記錄。

1. 建立並[將人員新增至靜態清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)。

1. [建立智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。

1. 在您於步驟二中建立之Smart Campaign的「智慧列示」中，尋找並新增&#x200B;**[!UICONTROL Member of List]**&#x200B;篩選器。

   ![](assets/three.png)

1. 尋找並選取您在步驟1中建立的清單。

   ![](assets/four.png)

1. 在流程中，尋找並新增&#x200B;**[!UICONTROL Change Program Status]**&#x200B;流程步驟。

   ![](assets/five.png)

1. 尋找並選取您的活動計畫。

   ![](assets/six.png)

1. 選擇您想要的狀態。

   ![](assets/seven.png)

1. 在[!UICONTROL Schedule]索引標籤中，按一下&#x200B;**[!UICONTROL Run Once]**。

   ![](assets/eight.png)

1. 選取「**[!UICONTROL Run Now]**」然後按一下「**[!UICONTROL Run]**」。

   ![](assets/nine.png)

1. 智慧型行銷活動執行後，成員會新增至方案，並將計入目標追蹤和事件上限推進計算中。
