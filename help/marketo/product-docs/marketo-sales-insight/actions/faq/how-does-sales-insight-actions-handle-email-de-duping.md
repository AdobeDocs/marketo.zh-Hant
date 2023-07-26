---
description: Sales Insight動作如何處理電子郵件重複資料刪除 — Marketo檔案 — 產品檔案
title: Sales Insight動作如何處理電子郵件重複資料刪除
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Sales Insight動作如何處理電子郵件重複資料刪除？ {#how-does-sales-insight-actions-handle-email-de-duping}

當您在 [上傳CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) 檔案放入銷售分析動作中，我們會在匯入前將所有類似的聯絡人合併到CSV中。

我們根據相似的電子郵件地址來執行此操作。 因此，如果有兩個相同的電子郵件地址，我們會將其合併為一個連絡人。

如果您稍後嘗試手動新增/上傳相同的連絡人，我們將不會合併它。

如果您嘗試新增資料庫中已存在的連絡人，我們將阻止您新增連絡人。
