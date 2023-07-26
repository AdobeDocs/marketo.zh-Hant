---
unique-page-id: 4719291
description: 設定預設人員姓氏和公司名稱 — Marketo檔案 — 產品檔案
title: 設定預設人員姓氏和公司名稱
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# 設定預設人員姓氏和公司名稱 {#set-default-person-last-name-and-company-name}

Salesforce的Leads和Contacts需要（最低）姓氏和公司名稱。 未完成的記錄將不會同步至Salesforce。 如果要同步部分記錄，您必須設定Marketo的預設值，以與Salesforce搭配使用。

1. 前往 **管理員** 並按一下 **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 按一下 **編輯同步選項**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 輸入 **預設人員姓氏** 和 **預設個人公司** 然後按一下 **儲存**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo只會在記錄最初同步至Salesforce時，而且僅當任一必要欄位為空白時，才指派預設值。

就是這樣！ 每次有人缺少姓氏和/或公司名稱時，Marketo都會新增預設值，因為它會將記錄同步過去。
