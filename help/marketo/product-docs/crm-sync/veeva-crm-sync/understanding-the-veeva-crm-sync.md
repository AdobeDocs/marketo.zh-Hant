---
description: 了解Veva CRM同步 — Marketo檔案 — 產品檔案
title: 了解Veeva CRM同步
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
source-git-commit: 884c9a27f3876ec3036f2f7187db30565cdd49a7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# 了解Veeva CRM同步 {#understanding-the-veeva-crm-sync}

只需幾個簡單步驟，即可輕鬆在Adobe Marketo Engage和Veeva CRM之間執行同步。

## 同步的運作方式 {#how-the-sync-works}

Marketo Engage會每天與Veeva CRM同步。 每次同步都需要一段時間，暫停5分鐘，然後再次開始。

>[!NOTE]
>
>第一次同步可能需要數小時甚至數天，因為Marketo Engage正從Veeva複製整個資料庫。 之後，每次同步通常需要幾分鐘（有時是幾秒），而且只同步已變更的資料。

![](assets/understanding-the-veeva-sync-1.png)

Veva和Marketo Engage之間的同步只對Person帳戶對象上的Contact欄位是雙向的。 在這些情況下，每當您在Veva或Marketo Engage中進行變更，您的更新都會反映在這兩個系統中。 所有其他同步只從VevaMarketo Engage。 按一下下方的連結，以取得每個連結的詳細資訊。

## Marketo Engage與Veeva之間同步的項目 {#what-is-synced-between-marketo-engage-and-veeva}

* [人員帳戶](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target=&quot;_blank&quot;}
* 使用者
* [呼叫和呼叫密鑰對象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
* [自訂物件](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}

## 須知 {#things-to-know}

* 此 [在VevaMarketo Engage中輸入的憑據](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target=&quot;_blank&quot;}可用來同步資料。 只會包含這些憑證可存取的資料。

* Veva CRM以force.com為基礎，而具有平台的豐富體驗Marketo Engage會繼承到此同步中。

* Veva CRM會顯示：銷售機會、聯繫人、帳戶（業務帳戶、機會、促銷活動和活動）。 不過，在與Marketo Engage同步時不支援這些設定。
