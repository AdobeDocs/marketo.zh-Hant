---
unique-page-id: 7515133
description: SFDC同步 — 合併銷售機會/聯繫人/人員 — Marketo文檔 — 產品文檔
title: SFDC同步 — 合併銷售機會/聯繫人/人員
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# SFDC同步：合併銷售機會/聯繫人/人員 {#sfdc-sync-merging-a-lead-contact-person}

有時最好只列出規則。 接下來：

* 合併兩個銷售機會時 **Salesforce**，一般同步會告訴Marketo，而銷售機會會自動合併為Marketo中的人員。
* 將兩個人合併 **Marketo** 實際調用與在Salesforce中將它們合併為銷售線索相同的流程。 它仍自動運作。
* 合併 **帶（人）進入聯繫人** 同樣的方法。 最後兩邊都只有一個接觸。
* 合併時，會加總預設分數。

>[!NOTE]
>
>合併3個銷售機會（人），每個分數為10，將產生1個銷售機會（人）的結果，分數為30。

* 從「成功記錄」中獲取衝突的欄位值。 （記錄=產生的銷售機會或聯繫人）
* 如果「失敗記錄」（即將消失的記錄）有價值，而勝出記錄沒有價值，我們將保留失敗記錄。 換句話說，「有些值比沒有值好。」
* 所有活動記錄項目皆會合併。

>[!NOTE]
>
>深入探討以取得 [合併Marketo人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
