---
unique-page-id: 2360370
description: 如何在同步前比對方案狀態和Salesforce促銷活動狀態 — Marketo檔案 — 產品檔案
title: 如何在同步之前匹配方案狀態和Salesforce促銷活動狀態
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 如何在同步之前匹配方案狀態和Salesforce促銷活動狀態 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

本文說明如何修正不相容的狀態錯誤，並在Marketo計畫和Salesforce促銷活動同步前對應狀態。

## 收到錯誤消息後，該做什麼 {#what-do-you-do-if-you-received-an-error-message}

如果您嘗試同步至包含銷售機會的現有Salesforce促銷活動，而促銷活動包含一或多個不相容的狀態，則會顯示錯誤訊息。 Marketo計畫與Salesforce行銷活動 *不會* 如果狀態不完全相符，則同步。

![](assets/image2015-7-22-9-3a23-3a29.png)

您可以從此錯誤訊息中選擇：

1. 從下拉式功能表（或）中選取要同步至的不同促銷活動
1. 您可以取消、修正狀態錯誤，並在錯誤修復後嘗試同步。 要修復狀態錯誤，請執行以下操作之一：

   * 登入Salesforce，移除或重新命名不相容的促銷活動成員狀態，以對應至與您的Marketo方案相關聯的管道類型所使用的Marketo方案狀態。
   * 修改Marketo中的方案狀態，以對應至您已設定的Salesforce促銷活動成員狀態。 這是Marketo管理功能。 如需詳細資訊，請參閱 [建立方案管道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
