---
unique-page-id: 3571833
description: Microsoft Dynamics Sync -Contact Sync - Marketo Docs —— 產品文檔
title: Microsoft Dynamics Sync -Contact Sync
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Microsoft Dynamics Sync:連絡同步{#microsoft-dynamics-sync-contact-sync}

您知道Market會將整個資料庫與Dynamics同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別處理Dynamics Contacts的一些詳細資訊。

## 這兩個系統之間的詳細資訊如何保持同步？{#how-are-details-kept-in-sync-between-the-two-systems}

聯繫人同步是雙向的。 如果您變更Dynamics中的聯絡人或Marketo中的人員，您的更新將反映在這兩個系統中。

## 如果同時對兩個系統中的同一欄位進行更改，該怎麼辦？ （資料衝突）{#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將贏得人們的青睞，而Dynamics將贏得人脈。 這是因為我們認為行銷部門對人有權威性，而官方的聯絡記錄系統則位於銷售(CRM)部門。

## 我可以使用Marketo建立連絡人嗎？{#can-i-create-a-contact-using-marketo}

是的。 [這是方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md)。

>[!NOTE]
>
>使用「將人員同步至Microsoft」流動動作（僅在觸發促銷活動中）時，銷售機會／連絡人會在Dynamics中即時建立。

## 我可以手動強制人員或聯繫人的同步嗎？{#can-i-manually-force-a-sync-of-a-person-or-a-contact}

否，自動化背景同步是同步Marketo和Dynamics之間更新的唯一方式。 [將人員同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)將不強制銷售線索同步。

## 哪些欄位將與Marketo同步？{#what-fields-will-sync-to-marketo}

您可以在設定期間選取要同步的欄位。 [](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)但Marketo只會同步您的Dynamics同步使用者可存取的欄位。

## Market會遵守Dynamics驗證規則嗎？{#will-marketo-respect-the-dynamics-validation-rules}

是的，如果發生衝突，則會將結果記錄在銷售線索活動日誌中。
