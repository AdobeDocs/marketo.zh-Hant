---
unique-page-id: 3571840
description: Microsoft Dynamics Sync — 使用者同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 使用者同步
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
source-git-commit: 7fcbaeda589682fdb5a75b89a0abd8661181566e
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Microsoft Dynamics同步：使用者同步 {#microsoft-dynamics-sync-user-sync}

您是否知道Marketo會使用Dynamics同步您的整個資料庫？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何具體處理Dynamics帳戶的一些詳細資料。

為進行整合，您需要專屬的Microsoft Dynamics CRM使用者。 我們稱此用戶為同步用戶。

## 如何讓兩個系統之間的使用者詳細資訊保持同步？ {#how-are-user-details-kept-in-sync-between-the-two-systems}

使用者同步是一種方式 — 從Dynamics同步至Marketo。 如果您在Dynamics中變更使用者，變更將會反映在Marketo中。

## 我可以使用Marketo建立使用者嗎？ {#can-i-create-an-user-using-marketo}

否. Marketo無法在Dynamics中建立使用者。

## 哪些欄位會同步至Marketo? {#which-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 進行設定。 但Marketo只會同步您的Dynamics同步使用者有權存取的欄位。
