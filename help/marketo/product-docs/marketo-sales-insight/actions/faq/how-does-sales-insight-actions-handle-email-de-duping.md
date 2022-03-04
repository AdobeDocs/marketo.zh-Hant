---
description: Sales Insight Actions如何處理電子郵件消除重複 — Marketo文檔 — 產品文檔
title: Sales Insight操作如何處理電子郵件去重複
hide: true
hidefromtoc: true
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Sales Insight操作如何處理電子郵件消除重複？ {#how-does-sales-insight-actions-handle-email-de-duping}

當你 [上載CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) 檔案到Sales Insight Actions中，在導入之前，我們將所有類似的聯繫人合併到CSV中。

我們根據類似的電子郵件地址執行此操作。 因此，如果有兩個相同的電子郵件地址，我們將它們合併為一個聯繫人。

如果您稍後嘗試手動添加/上載同一聯繫人，我們將不會合併它。

如果您嘗試添加資料庫中已有的聯繫人，我們將阻止您添加。
