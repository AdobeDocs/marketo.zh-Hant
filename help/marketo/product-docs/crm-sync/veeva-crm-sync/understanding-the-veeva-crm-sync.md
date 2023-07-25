---
description: 瞭解Veeva CRM同步 — Marketo檔案 — 產品檔案
title: 瞭解Veeva CRM Sync
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 瞭解Veeva CRM Sync {#understanding-the-veeva-crm-sync}

只要幾個簡單的步驟，就能輕鬆地在Adobe Marketo Engage和Veeva CRM之間執行同步。

## 同步如何運作 {#how-the-sync-works}

每天Marketo Engage與Veeva CRM同步。 每次同步都需要一些時間，會暫停5分鐘，然後再次開始。

>[!NOTE]
>
>首次同步可能需要數小時甚至數天，因為Marketo Engage正在從Veeva複製整個資料庫。 之後，每次同步通常需要數分鐘（有時是數秒）的時間，而且只會同步已變更的資料。

![](assets/understanding-the-veeva-sync-1.png)

Veeva和Marketo Engage之間的同步僅針對Person帳戶物件上的Contact欄位進行雙向同步。 在這些情況下，只要您在Veeva或Marketo Engage中進行變更，您的更新就會反映在這兩個系統中。 所有其他同步僅從Veeva到Marketo Engage。 按一下下列連結，以取得每個連結的詳細資料。

## Marketo Engage和Veeva之間同步的內容 {#what-is-synced-between-marketo-engage-and-veeva}

* [個人帳戶](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* 使用者
* [呼叫和呼叫關鍵物件](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [自訂物件](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## 須知事項 {#things-to-know}

* 此 [您在Veeva的Marketo Engage中輸入的認證](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} 用於同步資料。 只有這些認證有權存取的資料才會包括在內。

* Veeva CRM以force.com為基礎，此同步會繼承使用平台的豐富體驗Marketo Engage。

* Veeva CRM會顯示：銷售機會、聯絡人、帳戶（商業帳戶、商機、促銷活動和活動）。 不過，在與Marketo Engage同步時並不支援這些引數。
