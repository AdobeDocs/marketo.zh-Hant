---
unique-page-id: 37355758
description: 將成員新增至事件計畫 — Marketo檔案 — 產品檔案
title: 新增成員至事件程式
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# 新增成員至事件程式 {#adding-members-to-an-event-program}

本文僅適用於使用事件上限或事件目標的使用者。

>[!CAUTION]
>
>將人員清單直接匯入事件計畫時，這些記錄將無法計算在「目標追蹤」報表和「事件上限進度」報表中的實際註冊中。 請依照下列指示操作，以確保計算您的記錄。

1. 建立和 [將人員新增至靜態清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [建立智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. 在您於步驟二建立的Smart Campaign的「智慧列示」中，尋找並新增 **清單成員** 篩選。

   ![](assets/three.png)

1. 尋找並選取您在步驟1中建立的清單。

   ![](assets/four.png)

1. 在流量中，尋找並新增 **變更計畫狀態** 流程步驟。

   ![](assets/five.png)

1. 尋找並選取您的活動計畫。

   ![](assets/six.png)

1. 選擇您想要的狀態。

   ![](assets/seven.png)

1. 在「排程」標籤中，按一下 **執行一次**.

   ![](assets/eight.png)

1. 選取 **立即執行** 並按一下 **執行**.

   ![](assets/nine.png)

1. 智慧型行銷活動執行後，成員會新增至方案，並將計入目標追蹤和事件上限進展計算中。
