---
description: 瞭解 [!DNL Veeva] CRM Sync - Marketo檔案 — 產品檔案
title: 瞭解 [!DNL Veeva] CRM同步處理
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 瞭解[!DNL Veeva] CRM同步處理 {#understanding-the-veeva-crm-sync}

只要幾個簡單的步驟，就能輕鬆地在Adobe Marketo Engage和[!DNL Veeva] CRM之間執行同步。

## 同步如何運作 {#how-the-sync-works}

Marketo Engage每天都會與[!DNL Veeva] CRM同步。 每次同步都需要一些時間，暫停5分鐘，然後重新啟動。

>[!NOTE]
>
>首次同步處理可能需要數小時甚至數天的時間，因為Marketo Engage正在從[!DNL Veeva]複製整個資料庫。 之後，每個同步通常需要數分鐘（有時是數秒）的時間，而且只會同步已變更的資料。

![](assets/understanding-the-veeva-sync-1.png)

[!DNL Veeva]與Marketo Engage之間的同步只對個人帳戶物件上的連絡人欄位是雙向的。 在這些情況下，只要您在[!DNL Veeva]或Marketo Engage中進行變更，您的更新就會反映在兩個系統中。 所有其他同步僅從[!DNL Veeva]到Marketo Engage。 按一下下列連結，以取得每個專案的詳細資訊。

## Marketo Engage和[!DNL Veeva]之間同步的內容 {#what-is-synced-between-marketo-engage-and-veeva}

* [個人帳戶](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* 使用者
* [呼叫和呼叫主要物件](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [自訂物件](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## 須知 {#things-to-know}

* 您在Marketo Engage中為[輸入的 [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}認證可用來同步資料。 只有這些認證有權存取的資料才會包括在內。

* [!DNL Veeva] CRM以force.com為基礎，而Marketo Engage在平台上的豐富體驗繼承至此同步處理。

* Veeva CRM會顯示：銷售機會、聯絡人、帳戶、業務帳戶、機會、行銷活動和活動。 不過，在與Marketo Engage同步時並不支援這些功能。
