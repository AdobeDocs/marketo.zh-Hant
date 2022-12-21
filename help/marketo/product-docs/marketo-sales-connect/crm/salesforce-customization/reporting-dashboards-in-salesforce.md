---
unique-page-id: 14352464
description: Salesforce中的報表控制面板 — Marketo檔案 — 產品檔案
title: Salesforce中的報表控制面板
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Salesforce中的報表控制面板 {#reporting-dashboards-in-salesforce}

了解如何在下方設定控制面板。

## 開啟並按一下報表 {#open-and-click-report}

1. 選取 **任務和事件** 記錄類型。
1. 根據您需要的時間範圍和階層結構定義報表參數。
1. 新增篩選器以移除記錄至Salesforce的內部電子郵件(例如公司/帳戶不等於Marketo)。
1. 選取 **摘要** 報表格式。
1. 將「主體」、「已指派」和「Marketo銷售已點按/Marketo已檢視銷售」欄位新增至報表。
1. 按兩下 **添加公式** 欄位窗格中。
1. 將名稱添加到公式，選擇 **百分比** ，然後選取 **分組1**.
1. 選擇 **Marketo銷售人員已點按/Marketo已檢視銷售人員、** then **總和** （在摘要欄位中）。
1. 將除號加到公式，然後選取 **記錄計數** 在「摘要」欄位 —  _另存新檔_.

## 範本效能報表 {#template-performance-report}

1. 自訂「開啟並按一下」報表以包含下列欄位 —  _另存新檔_.

## 模板卷報告 {#template-volume-report}

1. 修改「範本績效報表」並加入「Marketo銷售範本不等於空白」篩選條件。
1. 移除「已點按Marketo銷售人員」欄位 —  _另存新檔_.

## 趨勢帳戶報表 {#trending-accounts-report}

1. 選擇「具有帳戶」記錄類型的活動。
1. 設定報表參數和欄位，如下所示 —  _另存新檔_.
