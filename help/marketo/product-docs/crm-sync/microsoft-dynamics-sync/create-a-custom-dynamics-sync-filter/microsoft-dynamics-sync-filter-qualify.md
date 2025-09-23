---
unique-page-id: 10092977
description: Microsoft Dynamics同步篩選器 — 合格 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步篩選器 — 合格
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步篩選器：合格 {#microsoft-dynamics-sync-filter-qualify}

當您想要在[!DNL Microsoft Dynamics]中將銷售機會轉換為聯絡人時，請務必使用此預設的資格程式。 然後，將其同步至Marketo。

## 轉換流程 {#the-conversion-process}

以下說明篩選器在轉換過程中的運作方式。

| 如果潛在客戶同步篩選器為： | 連絡人同步篩選器為： | 這是Marketo中的結果 |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Marketo中未同步任何專案 |
| [!UICONTROL True] | [!UICONTROL True] | 連絡人已在Marketo中同步 |
| [!UICONTROL False] | [!UICONTROL True] | 新的連絡人記錄是在Marketo中建立 |
| [!UICONTROL True] | [!UICONTROL False] | 在Marketo中更新[!DNL MS Dynamics]銷售機會資訊，但聯絡人記錄未同步 |

>[!CAUTION]
>
>我們僅支援現成可用的合格轉換程式。
