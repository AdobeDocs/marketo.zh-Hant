---
unique-page-id: 3571844
description: Microsoft Dynamics Sync -Opportunity Sync - Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 機會同步
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Microsoft Dynamics同步：機會同步 {#microsoft-dynamics-sync-opportunity-sync}

Dynamics同步的Marketo Engage功能非常強大。 以下是機會同步處理的所有詳細資料。

## 兩個系統之間的機會詳細資料如何保持同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

機會同步是單向的 — Dynamics與Marketo。 如果您在Dynamics中變更商機，您的更新將會反映在Marketo中。

## 我可以使用Marketo在Dynamics中建立機會嗎？ {#can-i-create-an-opportunity-in-dynamics-using-marketo}

否，您必須在Dynamics中建立機會，該機會會自動同步至Marketo。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可在安裝期間[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。

## 客戶/聯絡人如何與商機建立關聯？ {#how-is-an-account-contact-associated-with-an-opportunity}

聯絡人/帳戶可以兩種方式關聯至商機：

* 建立商機時，可以設定聯絡人（要聯絡的表單上的查詢欄位）和/或帳戶（要聯絡的表單上的查詢欄位）。 無論使用何種方法，這些值都會儲存在Dynamics的「潛在客戶(customerid)」欄位中。 此欄位未顯示在機會表單上，但可從設定新增。 此欄位只能包含1個值，可能是聯絡人或帳戶。 Marketo會執行下列動作：

   * 如果連絡人值已設定且帳戶留空，則Marketo會建立`opportunitycontactrole`並將商機的帳戶設定為連絡人的帳戶。 如果連絡人沒有帳戶，此欄位會保留空白。
   * 如果帳戶值已設定且聯絡人留空，Marketo將只會針對此帳戶設定該機會的帳戶。
   * 如果同時設定了這兩個值，Dynamics會挑選帳戶作為customerid的值，因此行為將與上述相同。


* 透過利害關係人： Dynamics會使用連線來連線機會，以便從機會建立頁面透過利害關係人進行聯絡。 為此，我們將為每個新利害關係人建立`opportunitycontactrole`記錄。
