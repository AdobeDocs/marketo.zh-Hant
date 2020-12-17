---
unique-page-id: 4719291
description: 設定預設人員姓氏和公司名稱——行銷人員檔案——產品檔案
title: 設定預設人員姓氏和公司名
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# 設定預設人員姓氏和公司名稱{#set-default-person-last-name-and-company-name}

Salesforce需要（最少）Lead和Contacts的姓氏和公司名稱。 不完整的記錄不會同步至Salesforce。 如果您想要同步部分記錄，您必須設定Marketo與Salesforce搭配使用的預設值。

1. 前往&#x200B;**Admin**，然後按一下&#x200B;**Salesforce**。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 按一下「編輯同步選項」 ****。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 輸入&#x200B;**預設人員姓**&#x200B;和**預設****人員公司** ，然後按一下&#x200B;**保存**。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo只會在記錄最初同步至Salesforce時指派預設值，而且只有在其中一個必填欄位空白時才指派。

就這樣！ 每次遺失姓氏和／或公司名稱時，Marketo會在記錄同步時新增預設值。
