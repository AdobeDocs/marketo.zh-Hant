---
unique-page-id: 3571848
description: Microsoft Dynamics同步 — 銷售機會同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 銷售機會同步
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft Dynamics同步：銷售機會同步 {#microsoft-dynamics-sync-lead-sync}

Marketo與Dynamics同步處理功能非常強大。 詳細資料如下：

## 兩個系統之間的詳細資料如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

同步是雙向的。 如果您變更Dynamics中的銷售機會或Marketo中的人員，您的更新將會反映在這兩個系統中。

>[!NOTE]
>
>刪除並不總是自動同步處理兩個方向。 另請參閱 [刪除潛在客戶或連絡人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## 如果兩個系統中的相同欄位同時發生變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將會贏得人員（銷售機會），而Dynamics將會贏得連絡人。 這是因為我們認為行銷部門是人員的權威，而聯絡人的官方記錄系統是在銷售(CRM)部門。

## 我可以使用Marketo在Dynamics中建立銷售機會嗎？ {#can-i-create-a-lead-in-dynamics-using-marketo}

是，請使用 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 流量動作。 如果銷售機會不存在，這會在Dynamics中建立銷售機會。 如果潛在客戶確實存在，則流程步驟將不會執行任何動作。

>[!NOTE]
>
>使用「將人員同步至Microsoft」流程動作時（僅適用於觸發促銷活動），系統會在Dynamics中即時建立銷售機會/聯絡人。

## 我可以手動強制將人員從Marketo同步到Dynamics中的潛在客戶嗎？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

否，自動背景同步是在Marketo和Dynamics之間同步更新的唯一方式。 此 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 流程動作不會強制同步潛在客戶。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 於設定期間。

## Marketo是否會遵守Dynamics驗證規則？ {#will-marketo-respect-the-dynamics-validation-rules}

是. 如果資料格式錯誤或遺失必要欄位資訊，同步處理將會失敗。 如果發生此情況，Marketo會將結果記錄在人員的活動記錄中。
