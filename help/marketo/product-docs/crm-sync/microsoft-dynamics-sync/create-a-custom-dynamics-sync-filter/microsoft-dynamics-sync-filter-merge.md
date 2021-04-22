---
unique-page-id: 10092969
description: Microsoft Dynamics Sync過濾器——合併-Marketo文檔——產品文檔
title: Microsoft Dynamics Sync篩選器——合併
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Microsoft Dynamics Sync篩選器：合併{#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合併銷售線索時，使用「兩個選項」類型-「同步」篩選器=「是」(TRUE)和「同步」篩選器=「否」(FALSE)。 合併兩個記錄時，結果會有所不同，具體取決於哪個記錄為True、哪個為False。

根據管理員定義的工作流程規則，銷售線索記錄會變成true或false，以判斷成功者。 成功記錄的同步篩選最終決定MS Dynamics記錄是否與Marketo同步。

當一個記錄是真的，一個是假的時候，它變得棘手。

| 如果丟失記錄的同步過濾器為： | 而成功記錄的同步篩選條件為： | 這是Marketo的結果 |
|---|---|---|
| True | True | 該得獎紀錄繼續與Marketo同步 |
| False | False | 成功記錄繼續與Marketo同步&#x200B;**not** |
| False | True | 獲勝的記錄將與Marketo同步 |
| True | False | 獲勝的記錄不會與Marketo同步 |
