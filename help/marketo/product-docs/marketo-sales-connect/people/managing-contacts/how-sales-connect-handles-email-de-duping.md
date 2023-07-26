---
unique-page-id: 14352514
description: Sales Connect如何處理電子郵件重複資料刪除 — Marketo檔案 — 產品檔案
title: Sales Connect如何處理電子郵件重複資料刪除
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Sales Connect如何處理電子郵件重複資料刪除 {#how-sales-connect-handles-email-de-duping}

當您在 [上傳CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) 檔案匯入Sales Connect後，我們會先合併CSV中所有類似的聯絡人，再進行匯入。

我們根據相似的電子郵件地址來執行此操作。 因此，如果有兩個相同的電子郵件地址，我們會將其合併為一個連絡人。

如果您稍後嘗試手動新增/上傳相同的連絡人，我們將不會合併它。

如果您嘗試新增資料庫中已存在的連絡人，我們將阻止您新增連絡人。
