---
unique-page-id: 3571840
description: Microsoft [!DNL Dynamics] Sync -User Sync - Marketo檔案 — 產品檔案
title: Microsoft [!DNL Dynamics] 同步 — 使用者同步
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Microsoft [!DNL Dynamics]同步：使用者同步 {#microsoft-dynamics-sync-user-sync}

您知道Marketo會將您的整個資料庫與[!DNL Dynamics]同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別處理[!DNL Dynamics]帳戶的一些詳細資料。

為了進行整合，您將需要專用的Microsoft [!DNL Dynamics] CRM使用者。 我們將此使用者稱為「同步處理使用者」。

## 這兩個系統之間的使用者詳細資料如何保持同步？ {#how-are-user-details-kept-in-sync-between-the-two-systems}

使用者同步是單向的 — [!DNL Dynamics]到Marketo。 如果您在[!DNL Dynamics]中變更使用者，這些變更將會反映在Marketo中。

## 我可以使用Marketo建立使用者嗎？ {#can-i-create-an-user-using-marketo}

不可以。 Marketo無法在[!DNL Dynamics]中建立使用者。

## 哪些欄位會同步至Marketo？ {#which-fields-will-sync-to-marketo}

您可在安裝期間[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)。 但Marketo將只會同步您的[!DNL Dynamics]同步使用者有權存取的欄位。
