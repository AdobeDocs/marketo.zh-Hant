---
unique-page-id: 3571848
description: Microsoft Dynamics Sync -Lead Sync - Marketo Docs —— 產品文檔
title: Microsoft Dynamics Sync -Lead Sync
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Microsoft Dynamics Sync:銷售線索同步{#microsoft-dynamics-sync-lead-sync}

Marketo to Dynamics sync功能強大。 以下是詳細資訊：

## 這兩個系統之間的詳細資訊如何保持同步？{#how-are-details-kept-in-sync-between-the-two-systems}

同步是雙向的。 如果您變更Dynamics中的銷售線索或Marketo中的人員，您的更新將反映在這兩個系統中。

>[!NOTE]
>
>刪除不總是自動在兩個方向同步。 請參閱[刪除銷售線索或聯繫人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md)。

## 如果同時對兩個系統中的同一欄位進行更改，該怎麼辦？ （資料衝突）{#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將贏得人（銷售機會），而Dynamics將贏得人脈。 這是因為我們認為行銷部門對人有權威性，而官方的聯絡記錄系統則位於銷售(CRM)部門。

## 我是否可使用Marketo在Dynamics中建立銷售機會？{#can-i-create-a-lead-in-dynamics-using-marketo}

是的，請使用「將人員同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流」操作。 [如果銷售線索不存在，這將在Dynamics中建立銷售線索。 如果銷售線索存在，流程步驟將不執行任何操作。

>[!NOTE]
>
>使用「將人員同步至Microsoft」流動動作（僅在觸發促銷活動中）時，銷售機會／連絡人會在Dynamics中即時建立。

## 我是否可手動強制Market與Dynamics中的銷售線索同步？{#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

否，自動化背景同步是同步Marketo和Dynamics之間更新的唯一方式。 [將人員同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流動操作不會強制銷售線索同步。

## 哪些欄位將與Marketo同步？{#what-fields-will-sync-to-marketo}

您可以在設定期間選取要同步的欄位。[](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)

## Market會遵守Dynamics驗證規則嗎？{#will-marketo-respect-the-dynamics-validation-rules}

是的。 如果資料格式錯誤或遺失必要欄位資訊，同步將會失敗。 Marketo會在發生此情況時，將結果記錄在人員的活動記錄中。
