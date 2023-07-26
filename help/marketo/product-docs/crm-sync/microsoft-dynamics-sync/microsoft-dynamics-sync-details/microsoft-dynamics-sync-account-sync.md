---
unique-page-id: 3571836
description: Microsoft Dynamics同步 — 帳戶同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 帳戶同步
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics同步：帳戶同步 {#microsoft-dynamics-sync-account-sync}

您知道Marketo會將您的整個資料庫與Dynamics同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別處理Dynamics帳戶的部分細節。

## 資訊會以何種方式同步？ {#which-way-does-the-information-sync}

只有一種方式：從Dynamics到Marketo。

## 更新如何運作？ {#how-do-the-updates-work}

如果您更新Marketo中連絡人的「帳戶」欄位，這會變更Marketo中屬於該帳戶的所有連絡人的值。 它不會同步至Dynamics。 不過，下次在Dynamics中更新該帳戶時，變更將會覆寫Marketo中的所有帳戶資訊。

## 我可以使用Marketo建立帳戶嗎？ {#can-i-create-an-account-using-marketo}

否. Marketo無法在Dynamics中建立帳戶。

## 哪些欄位會同步至Marketo？ {#which-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 於設定期間。 但Marketo只會同步處理您的Dynamics同步使用者有權存取的欄位。

## Dynamics中帳戶欄位的變更是否會導致每個連絡人的變更資料值活動記錄？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

大部份是這樣。 但是，如果某個帳戶擁有超過5,000個連絡人，而該帳戶上的欄位在Dynamics中發生變更，我們會同步處理變更，但不會記錄5,000多個連絡人的活動。
