---
unique-page-id: 2360370
description: 如何在同步前匹配計畫狀態和Salesforce促銷活動狀態-Marketo文檔——產品文檔
title: 如何在同步前匹配方案狀態和Salesforce促銷活動狀態
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 如何在同步{#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}之前匹配程式狀態和Salesforce促銷活動狀態

本文說明如何在Marketo計畫和Salesforce促銷活動同步之前修正不相容的狀態錯誤並對應狀態。

## 如果您收到錯誤訊息{#what-do-you-do-if-you-received-an-error-message}，該怎麼辦

如果您嘗試同步至包含銷售機會且促銷活動包含一或多個不相容狀態的現有Salesforce促銷活動，則會顯示錯誤訊息。 如果狀態不完全相符，則「Marketo計畫」和「Salesforce促銷活動」*將不會*&#x200B;同步。

![](assets/image2015-7-22-9-3a23-3a29.png)

從此錯誤訊息中，您可以選擇：

1. 從下拉式選單(OR)選取要同步至的不同促銷活動
1. 您可以取消、修正狀態錯誤，並在錯誤修復後嘗試同步。 要修正狀態錯誤，請執行下列操作之一：

   * 登入Salesforce並移除或重新命名不相容的促銷活動成員狀態，以對應至與您的「Marketo計畫」相關聯之頻道類型所使用的「Marketo計畫狀態」。
   * 修改Marketo的「方案狀態」，以對應至您已有的Salesforce促銷活動成員狀態。 這是Marketo管理員的職能。 有關詳細資訊，請參閱[建立程式通道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)。
