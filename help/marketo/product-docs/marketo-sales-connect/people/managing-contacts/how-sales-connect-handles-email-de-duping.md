---
unique-page-id: 14352514
description: Sales Connect如何處理電子郵件去重複化 — Marketo檔案 — 產品檔案
title: Sales Connect如何處理電子郵件去重複化
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Sales Connect如何處理電子郵件去重複化 {#how-sales-connect-handles-email-de-duping}

當你 [上傳CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) 檔案放入Sales Connect中後，我們會在匯入之前，在CSV中合併所有類似的聯絡人。

我們是根據類似電子郵件地址執行此操作。 因此，如果有兩個相同的電子郵件地址，我們會將它們合併為一個聯絡人。

如果您稍後嘗試手動新增/上傳相同的連絡人，我們不會合併該連絡人。

如果您嘗試添加資料庫中已有的聯繫人，我們將阻止您添加該聯繫人。
