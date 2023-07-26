---
unique-page-id: 10092969
description: Microsoft Dynamics同步篩選器 — 合併 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步篩選器 — 合併
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics同步篩選器：合併 {#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合併銷售機會使用兩個選項型別 — 同步篩選器=是(TRUE)和同步篩選器=否(FALSE)。 合併兩個記錄時，結果會因記錄為True和記錄為False而有所不同。

根據管理員定義的工作流程規則，潛在客戶記錄會變成true或false以判斷獲勝者。 成功記錄的同步篩選最終將決定MS Dynamics記錄是否與Marketo同步。

當一筆記錄為真而一筆記錄為假時，就會變得棘手。

| 如果遺失記錄的同步處理篩選為： | 而且成功記錄的同步處理篩選條件為： | 這是Marketo中的結果 |
|---|---|---|
| True | True | 成功記錄會繼續與Marketo同步 |
| False | False | 成功紀錄將繼續 **非** 與Marketo同步 |
| False | True | 成功記錄將與Marketo同步 |
| True | False | 成功記錄不會與Marketo同步 |
