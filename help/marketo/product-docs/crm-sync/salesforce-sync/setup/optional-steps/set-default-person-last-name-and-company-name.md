---
unique-page-id: 4719291
description: 設定預設人員姓氏和公司名稱 — Marketo檔案 — 產品檔案
title: 設定預設人員姓氏和公司名稱
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 13%

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

就是這樣！ 每次有人缺少姓氏和/或公司名稱時，Marketo都會新增預設值，因為它會將記錄同步過去。
