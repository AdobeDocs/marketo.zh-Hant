---
unique-page-id: 4719291
description: 設定預設人員姓氏和公司名稱 — Marketo檔案 — 產品檔案
title: 設定預設人員姓氏和公司名稱
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# 設定預設人員姓氏和公司名稱 {#set-default-person-last-name-and-company-name}

Salesforce要求其Lead和Contact的姓氏和公司名稱為（最低）。 不完整的記錄將不會同步到Salesforce。 如果要同步部分記錄，必須設定預設值，使Marketo能與Salesforce搭配使用。

1. 前往 **管理** 按一下 **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 按一下 **編輯同步選項**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 輸入 **預設人員姓氏** 和 **預設人員公司** 然後按一下 **儲存**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo只會在記錄最初同步至Salesforce時指派預設值，且僅限於其中一個必填欄位為空時。

就這樣！ 每次有人遺失姓氏和/或公司名稱時，Marketo都會新增預設值，同步記錄。
