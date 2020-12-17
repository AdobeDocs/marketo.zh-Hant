---
unique-page-id: 2360370
description: 如何在同步前比對計畫狀態和Salesforce促銷活動狀態——行銷人員檔案——產品檔案
title: 如何在同步前匹配方案狀態和Salesforce促銷活動狀態
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# 如何在同步{#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}之前匹配程式狀態和Salesforce促銷活動狀態

本文說明如何修正不相容的狀態錯誤，並在Marketo Program和Salesforce Campaign同步之前對應狀態。

## 如果您收到錯誤訊息{#what-do-you-do-if-you-received-an-error-message}，該怎麼辦

如果您嘗試同步至包含銷售機會且促銷活動包含一或多個不相容狀態的現有Salesforce促銷活動，則會顯示錯誤訊息。 如果狀態不完全相符，Marketo程式和Salesforce促銷活動&#x200B;*將不會同步。*

![](assets/image2015-7-22-9-3a23-3a29.png)

從此錯誤訊息中，您可以選擇：

1. 從下拉式選單(OR)選取要同步至的不同促銷活動
1. 您可以取消、修正狀態錯誤，並在錯誤修復後嘗試同步。 要修正狀態錯誤，請執行下列操作之一：

   * 登入Salesforce並移除或重新命名不相容的促銷活動成員狀態，以對應至與您的Marketo Program相關聯之渠道類型所使用的Marketo Program狀態。
   * 修改Market中的「方案狀態」，以對應至您現有的Salesforce促銷活動成員狀態。 這是行銷人員管理功能。 有關詳細資訊，請參閱[建立程式通道](../../../../../product-docs/administration/tags/create-a-program-channel.md)。

