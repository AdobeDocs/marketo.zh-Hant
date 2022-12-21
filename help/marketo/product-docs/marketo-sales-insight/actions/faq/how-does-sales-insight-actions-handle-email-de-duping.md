---
description: Sales Insight Actions如何處理電子郵件去重複化 — Marketo檔案 — 產品檔案
title: Sales Insight Actions如何處理電子郵件去重複化
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Sales Insight Actions如何處理電子郵件去重複化？ {#how-does-sales-insight-actions-handle-email-de-duping}

當你 [上傳CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) 檔案合併至「銷售分析動作」中，我們會在匯入之前，在CSV中合併所有類似的聯絡人。

我們是根據類似電子郵件地址執行此操作。 因此，如果有兩個相同的電子郵件地址，我們會將它們合併為一個聯絡人。

如果您稍後嘗試手動新增/上傳相同的連絡人，我們不會合併該連絡人。

如果您嘗試添加資料庫中已有的聯繫人，我們將阻止您添加該聯繫人。
