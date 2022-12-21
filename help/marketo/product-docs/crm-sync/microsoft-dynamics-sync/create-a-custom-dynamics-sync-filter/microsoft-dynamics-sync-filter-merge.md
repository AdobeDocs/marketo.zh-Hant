---
unique-page-id: 10092969
description: Microsoft Dynamics同步篩選器 — 合併 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步篩選器 — 合併
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics同步篩選器：合併 {#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合併銷售機會時使用「兩個選項」類型 — 同步篩選器=是(TRUE)和同步篩選器=否(FALSE)。 合併兩條記錄時，結果會有所不同，具體取決於哪條記錄為True、哪條為False。

銷售機會記錄會根據管理員定義的工作流程規則變成true或false，以決定獲勝者。 成功記錄的同步篩選器最終決定MS Dynamics記錄是否與Marketo同步。

當一條記錄是真的，一條是假的時候，它就會變得棘手。

| 如果丟失記錄的同步篩選器為： | 成功記錄的同步篩選器為： | 這是Marketo的結果 |
|---|---|---|
| True | True | 成功記錄會繼續與Marketo同步 |
| False | False | 成功記錄將繼續 **not** 與Marketo同步 |
| False | True | 成功記錄將與Marketo同步 |
| True | False | 成功記錄不會與Marketo同步 |
