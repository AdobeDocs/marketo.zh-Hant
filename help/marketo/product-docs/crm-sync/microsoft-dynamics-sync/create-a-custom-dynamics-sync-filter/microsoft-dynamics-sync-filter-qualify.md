---
unique-page-id: 10092977
description: Microsoft Dynamics Sync篩選——資格-Marketo文檔——產品文檔
title: Microsoft Dynamics Sync篩選器-Qualify
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Microsoft Dynamics Sync篩選器：限定{#microsoft-dynamics-sync-filter-qualify}

當您想要在Microsoft Dynamics中將銷售線索轉換為聯繫人時，請務必使用此預設的「限定」流程。 然後，將它同步到Marketo。

## 轉換程式{#the-conversion-process}

以下是篩選器在轉換過程中的運作方式。

| 如果銷售線索同步篩選器為： | 而連絡同步篩選器為： | 這是Marketo的結果 |
|---|---|---|
| False | False | Marketo沒有同步 |
| True | True | 聯絡人在Marketo |
| False | True | 在Marketo建立新的聯絡記錄 |
| True | False | MS Dynamics會更新Marketo的銷售線索資訊，但聯絡記錄未同步 |

>[!CAUTION]
>
>我們僅支援現成可用的Qualify轉換程式。
