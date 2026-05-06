---
unique-page-id: 14352514
description: 瞭解Sales Connect如何處理電子郵件重複資料刪除。 瞭解同步時如何合併或處理重複的連絡人。
title: Sales Connect 如何處理刪除重複電子郵件的作業
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 6%

---

# [!DNL Sales Connect]如何處理電子郵件重複資料刪除 {#how-sales-connect-handles-email-de-duping}

當您[將CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)檔案上傳到[!DNL Sales Connect]時，我們會在匯入發生之前合併CSV中的所有類似聯絡人。

我們根據相似的電子郵件地址來執行此操作。 因此，如果有兩個相同的電子郵件地址，我們會將其合併為一個連絡人。

如果您稍後嘗試手動新增/上傳相同的連絡人，我們將不會合併它。

如果您嘗試新增資料庫中已存在的連絡人，我們將阻止您新增連絡人。
