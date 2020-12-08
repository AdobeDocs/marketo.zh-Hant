---
unique-page-id: 14352514
description: Sales Connect如何處理電子郵件去重複化——行銷檔案——產品檔案
title: Sales Connect如何處理電子郵件去重複化
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Sales Connect如何處理電子郵件去重複化 {#how-sales-connect-handles-email-de-duping}

當您將CSV檔案 [上傳至Sales Connect時](http://docs.marketo.com/x/VADb) ，我們會在匯入之前，將所有類似CSV的連絡人合併。

我們根據類似的電子郵件地址來執行此動作。 因此，如果有兩個相同的電子郵件地址，我們會將它們合併為一個聯絡人。

如果您稍後嘗試手動新增／上傳相同的連絡人，我們將不會合併該連絡人。

如果您嘗試新增資料庫中已有的連絡人，我們會禁止您新增。

