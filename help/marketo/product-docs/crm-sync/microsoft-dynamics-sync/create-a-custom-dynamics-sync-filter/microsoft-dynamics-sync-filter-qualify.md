---
unique-page-id: 10092977
description: Microsoft Dynamics同步篩選器 — 資格 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步篩選器 — 合格
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics同步篩選器：合格 {#microsoft-dynamics-sync-filter-qualify}

當您想要在Microsoft Dynamics中將銷售機會轉換為聯絡人時，請務必使用此預設的資格程式。 然後，將其同步至Marketo。

## 轉換過程 {#the-conversion-process}

以下說明篩選器在轉換過程中的運作方式。

| 如果潛在客戶同步篩選器為： | 連絡人同步篩選器為： | 這是Marketo中的結果 |
|---|---|---|
| False | False | Marketo中未同步任何專案 |
| True | True | 連絡人已在Marketo中同步 |
| False | True | 新的連絡人記錄建立於Marketo |
| True | False | MS Dynamics會更新Marketo中的銷售機會資訊，但聯絡人記錄並未同步 |

>[!CAUTION]
>
>我們僅支援現成可用的資格轉換程式。
