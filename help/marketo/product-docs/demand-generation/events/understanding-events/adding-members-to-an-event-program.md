---
unique-page-id: 37355758
description: 新增成員至事件方案 — Marketo檔案 — 產品檔案
title: 向事件程式添加成員
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# 向事件程式添加成員 {#adding-members-to-an-event-program}

本文僅適用於使用事件上限或事件目標的使用者。

>[!CAUTION]
>
>將人員清單直接匯入「事件方案」將防止這些記錄計入「目標追蹤」報表和「事件上限進展」報表中的實際註冊。 請依照下列指示，確保記錄經過計算。

1. 建立和 [將人員新增至靜態清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [建立智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. 在您於步驟二建立的智慧型促銷活動的智慧清單中，尋找並新增 **清單成員** 篩選。

   ![](assets/three.png)

1. 尋找並選取您在步驟一中建立的清單。

   ![](assets/four.png)

1. 在「流量」中，尋找並新增 **更改程式狀態** 流程步驟。

   ![](assets/five.png)

1. 查找並選擇您的事件方案。

   ![](assets/six.png)

1. 選擇您想要的狀態。

   ![](assets/seven.png)

1. 在「排程」標籤中，按一下 **執行一次**.

   ![](assets/eight.png)

1. 選擇 **立即運行** 按一下 **執行**.

   ![](assets/nine.png)

1. 智慧型促銷活動執行後，會將成員新增至方案，並計入目標追蹤和事件上限進度計算。
