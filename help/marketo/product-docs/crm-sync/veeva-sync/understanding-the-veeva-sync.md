---
description: 瞭解Veeva同步 — Marketo文檔 — 產品文檔
title: 瞭解Veeva同步
hide: true
hidefromtoc: true
source-git-commit: c36b9206494c14a52937fa787a37601eaf6f4bd4
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# 瞭解Veeva同步 {#understanding-the-veeva-sync}

只需幾個簡單的步驟，便可在Adobe Marketo Engage和Veeva CRM之間輕鬆同步。

## 同步的工作原理 {#how-the-sync-works}

Marketo Engage與Veeva CRM全天候同步。 每次同步都需要一段時間，暫停5分鐘，然後重新開始。

>[!NOTE]
>
>第一次同步可能需要數小時甚至數天，因為Marketo Engage正在從Veeva複製整個資料庫。 之後，每次同步通常需要幾分鐘（有時是幾秒），並且只同步已更改的資料。

![](assets/understanding-the-veeva-sync-1.png)

Veva和Marketo Engage之間的同步僅對「人員」帳戶對象上的「聯繫人」欄位是雙向的。 在這些情況下，只要您在Veeva或Marketo Engage中進行更改，您的更新就會反映在兩個系統中。 所有其它同步僅從Veeva到Marketo Engage。 按一下以下連結以瞭解每個連結的詳細資訊。

## Marketo和維娃之間的同步內容 {#what-is-synced-between-marketo-and-veeva}

人員帳戶用戶調用和調用密鑰對象自定義對象

## 要知道的事 {#things-to-know}

* 您在Marketo Engage中為Veeva輸入的憑據用於同步資料。 將只包括那些憑據有權訪問的資料。

* Veeva CRM是基於force.com的，與該平台的豐富體驗Marketo Engage繼承到此同步中。

* Veeva CRM顯示：銷售線索、聯繫人、客戶（業務帳戶、機會、市場活動和活動）。 但是，在與Marketo Engage同步時不支援它們。
