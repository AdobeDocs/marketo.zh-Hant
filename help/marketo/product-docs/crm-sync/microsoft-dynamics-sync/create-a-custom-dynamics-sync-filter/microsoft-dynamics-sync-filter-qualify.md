---
unique-page-id: 10092977
description: Microsoft Dynamics同步篩選器 — 資格 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步篩選器 — 合格
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Microsoft Dynamics同步篩選器：合格 {#microsoft-dynamics-sync-filter-qualify}

在Microsoft Dynamics中，如果要將銷售機會轉換為聯繫人，請務必使用此預設的合格流程。 然後，將其同步至Marketo。

## 轉換程式 {#the-conversion-process}

以下是轉換過程中篩選器的運作方式。

| 如果銷售機會同步篩選器為： | 聯繫人同步過濾器為： | 這是Marketo的結果 |
|---|---|---|
| False | False | 未同步任何項目Marketo |
| True | True | 連絡人已同步至Marketo |
| False | True | 已在Marketo中建立新的聯絡記錄 |
| True | False | MS Dynamics更新Marketo中的銷售機會資訊，但未同步連絡記錄 |

>[!CAUTION]
>
>我們僅支援現成可用的合格轉換程式。
