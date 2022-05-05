---
description: 瞭解Veeva CRM同步 — Marketo文檔 — 產品文檔
title: 瞭解Veeva CRM同步
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# 瞭解Veeva CRM同步 {#understanding-the-veeva-crm-sync}

只需幾個簡單的步驟，便可在Adobe Marketo Engage和Veeva CRM之間輕鬆同步。

## 同步的工作原理 {#how-the-sync-works}

Marketo Engage與Veeva CRM全天候同步。 每次同步都需要一段時間，暫停5分鐘，然後重新開始。

>[!NOTE]
>
>第一次同步可能需要數小時甚至數天，因為Marketo Engage正在從Veeva複製整個資料庫。 之後，每次同步通常需要幾分鐘（有時是幾秒），並且只同步已更改的資料。

![](assets/understanding-the-veeva-sync-1.png)

Veva和Marketo Engage之間的同步僅對「人員」帳戶對象上的「聯繫人」欄位是雙向的。 在這些情況下，只要您在Veeva或Marketo Engage中進行更改，您的更新就會反映在兩個系統中。 所有其它同步僅從Veeva到Marketo Engage。 按一下以下連結以瞭解每個連結的詳細資訊。

## Marketo Engage和維娃之間同步的內容 {#what-is-synced-between-marketo-engage-and-veeva}

* [人員帳戶](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target=&quot;_blank&quot;
* 用戶
* [調用和調用密鑰對象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;
* [自定義對象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/veeva-crm-custom-object-sync.md){target=&quot;_blank&quot;

## 要知道的事 {#things-to-know}

* 的 [在Marketo Engage中輸入的憑據](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target=&quot;_blank&quot;}用於同步資料。 將只包括那些憑據有權訪問的資料。

* Veeva CRM是基於force.com的，與該平台的豐富體驗Marketo Engage繼承到此同步中。

* Veeva CRM顯示：銷售線索、聯繫人、客戶（業務帳戶、機會、市場活動和活動）。 但是，在與Marketo Engage同步時不支援它們。
