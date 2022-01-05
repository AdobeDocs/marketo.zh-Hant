---
unique-page-id: 3571833
description: Microsoft Dynamics Sync — 連絡人同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 聯繫人同步
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
source-git-commit: 7fcbaeda589682fdb5a75b89a0abd8661181566e
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Microsoft Dynamics同步：聯繫人同步 {#microsoft-dynamics-sync-contact-sync}

您是否知道Marketo會使用Dynamics同步您的整個資料庫？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是有關Marketo如何具體處理Dynamics聯繫人的一些詳細資訊。

## 如何使這兩個系統之間的詳細資訊保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

接觸同步是雙向的。 如果您在Dynamics中變更連絡人或在Marketo中變更人員，您的更新將會反映在兩個系統中。

## 如果同時對兩個系統中的相同欄位進行變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這是罕見的，但Marketo將贏得人民，動力將贏得人脈。 這是因為我們認為營銷部門對人具有權威性，而官方的聯繫記錄系統是銷售(CRM)部門。

## 我可以使用Marketo建立連絡人嗎？ {#can-i-create-a-contact-using-marketo}

是。 [以下是如何](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>使用「將人員同步至Microsoft」流量動作時（僅限於觸發促銷活動中），銷售機會/連絡人將在Dynamics中即時建立。

## 我可以手動強制人員或聯絡人同步嗎？ {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

否，自動背景同步是在Marketo和Dynamics之間同步更新的唯一方式。 此 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 不會強制銷售線索同步。

## 哪些欄位會同步至Marketo? {#what-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 進行設定。 但Marketo只會同步您的Dynamics同步使用者有權存取的欄位。

## Marketo會遵守Dynamics驗證規則嗎？ {#will-marketo-respect-the-dynamics-validation-rules}

是，如果發生衝突，則會將結果記錄在銷售機會活動日誌中。
