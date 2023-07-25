---
unique-page-id: 7515133
description: SFDC同步 — 合併銷售機會/聯絡人/人員 — Marketo檔案 — 產品檔案
title: SFDC同步 — 合併銷售機會/連絡人/人員
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# SFDC同步：合併銷售機會/連絡人/人員 {#sfdc-sync-merging-a-lead-contact-person}

有時最好只列出規則。 接下來是：

* 當您合併兩個潛在客戶時 **Salesforce**，一般sync會告知Marketo，而銷售機會會自動以Marketo中的人員身分合併。
* 合併兩個人員 **Marketo** 實際上會叫用與在Salesforce中合併潛在客戶相同的程式。 仍可自動運作。
* 合併 **潛在客戶（人員）進入聯絡人** 運作方式相同。 您最後在兩邊各有一個接觸點。
* 合併時，會加總預設分數。

>[!NOTE]
>
>合併每個分數為10的3個銷售機會（人員），會產生1個銷售機會（人員）的結果，分數為30。

* 衝突的欄位值取自「成功記錄」。 （記錄=產生的潛在客戶或連絡人）
* 如果「失敗記錄」（正在消失的記錄）有一個值，且成功記錄沒有值，我們會保留失敗記錄。 換句話說，「有值總比沒有值好。」
* 所有活動記錄專案都會合併。

>[!NOTE]
>
>深入瞭解，以瞭解更多關於 [在Marketo中合併人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
