---
unique-page-id: 3571833
description: Microsoft Dynamics Sync — 連絡人同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 連絡人同步
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Microsoft Dynamics同步：連絡人同步 {#microsoft-dynamics-sync-contact-sync}

您知道Marketo會將您的整個資料庫與Dynamics同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別處理Dynamics聯絡人的部分細節。

## 兩個系統之間的詳細資料如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

連絡人同步是雙向的。 如果您變更Dynamics中的連絡人或Marketo中的人員，您的更新將會反映在這兩個系統中。

## 如果兩個系統中的相同欄位同時發生變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將贏得人心，而Dynamics將贏得連絡人。 這是因為我們認為行銷部門是人員的權威，而聯絡人的官方記錄系統是在銷售(CRM)部門。

## 我可以使用Marketo建立連絡人嗎？ {#can-i-create-a-contact-using-marketo}

是. [方法如下](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>使用「將人員同步至Microsoft」流程動作時（僅適用於觸發促銷活動），系統會在Dynamics中即時建立銷售機會/聯絡人。

## 我可以手動強制同步處理人員或連絡人嗎？ {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

不會，自動背景同步是在Marketo和Dynamics之間同步更新的唯一方法。 此 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 不會強制同步處理銷售機會。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 於設定期間。 但Marketo只會同步處理您的Dynamics同步使用者有權存取的欄位。

## Marketo是否會遵守Dynamics驗證規則？ {#will-marketo-respect-the-dynamics-validation-rules}

是，如果發生衝突，則會將結果記錄在潛在客戶活動記錄中。
