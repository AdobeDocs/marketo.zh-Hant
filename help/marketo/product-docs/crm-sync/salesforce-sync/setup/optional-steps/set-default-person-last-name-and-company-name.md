---
unique-page-id: 4719291
description: 瞭解如何設定Salesforce同步的預設人員姓氏和公司名稱。 使用管理和同步選項，讓部分記錄與預設值同步。
title: 設定預設人員姓氏和公司名稱
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/pq4XPfiwO1UemSmg3edhJgWWmvR-mx4Q3udff9xzWt0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 137
ht-degree: 12%

---

# 設定預設人員姓氏和公司名稱 {#set-default-person-last-name-and-company-name}

[!DNL Salesforce]需要（最少）潛在客戶與聯絡人的姓氏與公司名稱。 未完成的記錄將不會同步至[!DNL Salesforce]。 如果您想要同步部分記錄，您必須設定Marketo的預設值，才能與[!DNL Salesforce]搭配使用。

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;並按一下&#x200B;**[!DNL Salesforce]**。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 按一下「**[!UICONTROL Edit Sync Options]**」。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 輸入&#x200B;**[!UICONTROL Default person last name]**&#x200B;和&#x200B;**[!UICONTROL Default person company]**，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage只會在記錄最初同步至Salesforce時，而且僅在任一必要欄位空白時指派預設值。

每次人員遺失姓氏或公司名稱時，Marketo都會新增預設值，以便透過該處同步記錄。
