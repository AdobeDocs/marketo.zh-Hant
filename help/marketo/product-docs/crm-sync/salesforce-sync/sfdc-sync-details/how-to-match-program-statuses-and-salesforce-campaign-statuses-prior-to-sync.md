---
unique-page-id: 2360370
description: 如何在同步之前比對方案狀態和Salesforce行銷活動狀態 — Marketo檔案 — 產品檔案
title: 如何在同步之前讓方案狀態和 Salesforce 行銷活動狀態相符
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 5%

---

# 如何在同步之前比對方案狀態和[!DNL Salesforce]行銷活動狀態 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

本文說明如何修正不相容的狀態錯誤，並在Marketo程式和[!DNL Salesforce] Campaign同步處理之前對應狀態。

## 如果您收到錯誤訊息，該怎麼做 {#what-do-you-do-if-you-received-an-error-message}

如果您嘗試同步至包含銷售機會的現有[!DNL Salesforce]行銷活動，而該行銷活動包含一或多個不相容的狀態，則會顯示錯誤訊息。 如果狀態不完全相符，Marketo方案與[!DNL Salesforce]行銷活動&#x200B;*將不會*&#x200B;同步。

![](assets/image2015-7-22-9-3a23-3a29.png)

從這個錯誤訊息中，您可以選擇：

1. 從下拉式選單選取要同步到的其他行銷活動，或
1. 您可以取消、修正狀態錯誤，並在錯誤修復後嘗試同步。 若要修正狀態錯誤，請執行下列任一項作業：

   * 登入Salesforce，並移除或重新命名不相容的「行銷活動成員狀態」，以對應至與您的Marketo方案相關聯的管道型別所使用的Marketo方案狀態。
   * 修改Marketo中的方案狀態，以對應至您已就緒的Salesforce促銷活動會員狀態。 這是Marketo管理員功能。 如需詳細資訊，請參閱[建立方案頻道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}。
