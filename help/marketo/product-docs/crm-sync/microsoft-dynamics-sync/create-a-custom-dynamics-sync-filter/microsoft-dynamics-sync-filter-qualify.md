---
unique-page-id: 10092977
description: Microsoft Dynamics Sync篩選器——資格——行銷人員文檔——產品文檔
title: Microsoft Dynamics Sync篩選器-Qualify
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Microsoft Dynamics Sync篩選器：符合資格 {#microsoft-dynamics-sync-filter-qualify}

當您想要在Microsoft Dynamics中將銷售線索轉換為聯繫人時，請務必使用此預設的「限定」流程。 然後，將它同步至Marketo。

## 轉換程式 {#the-conversion-process}

以下是篩選器在轉換過程中的運作方式。

| 如果銷售線索同步篩選器為： | 而連絡同步篩選器為： | 這是Marketo的成果 |
|---|---|---|
| False | False | Marketo中沒有同步項目 |
| True | True | 此連絡人在Marketo中同步 |
| False | True | 在Marketo中建立新的連絡記錄 |
| True | False | MS Dynamics會更新Marketo中的銷售機會資訊，但不會同步連絡記錄 |

>[!CAUTION]
>
>我們僅支援現成可用的Qualify轉換程式。

