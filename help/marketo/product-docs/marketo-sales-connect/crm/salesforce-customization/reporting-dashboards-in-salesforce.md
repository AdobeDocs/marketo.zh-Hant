---
unique-page-id: 14352464
description: Salesforce中的報告儀表板 — Marketo檔案 — 產品檔案
title: Salesforce中的報告儀表板
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Salesforce中的報告儀表板 {#reporting-dashboards-in-salesforce}

瞭解如何在下方設定儀表板。

## 開啟並按一下報表 {#open-and-click-report}

1. 選取&#x200B;**[!UICONTROL Tasks and Events]**&#x200B;記錄型別。
1. 根據您想要的時間範圍和階層結構定義報表引數。
1. 新增篩選器以移除記錄至[!DNL Salesforce]的內部電子郵件(例如不等於Marketo的公司/帳戶)。
1. 選取&#x200B;**[!UICONTROL Summary]**&#x200B;報告格式。
1. 將「主旨」、「已指派」和「已點選Marketo銷售」/「已檢視Marketo銷售」欄位新增至報表。
1. 在[欄位]窗格中連按兩下&#x200B;**[!UICONTROL Add Formula]**。
1. 新增名稱至公式，以格式選取&#x200B;**[!UICONTROL Percent]**，然後選取&#x200B;**[!UICONTROL Grouping 1]**。
1. 在[摘要]欄位中選取&#x200B;**[!UICONTROL Marketo Sales Clicked/Marketo Sales Viewed]**，然後選取&#x200B;**[!UICONTROL Sum]**。
1. 在公式中加入除號，然後在[摘要]欄位中選取&#x200B;**[!UICONTROL Record Count]** - _另存新檔_。

## 範本效能報表 {#template-performance-report}

1. 自訂「開啟並點按」報告以包含以下欄位 — _另存新檔_。

## 範本磁碟區報告 {#template-volume-report}

1. 修改範本效能報表並加入篩選器：「Marketo銷售範本不等於空白」。
1. 移除Marketo銷售點選欄位 — _另存新檔_。

## 趨勢帳戶報表 {#trending-accounts-report}

1. 選取具有帳戶記錄型別的活動。
1. 設定報表引數和欄位，如下所示 — _另存新檔_。
