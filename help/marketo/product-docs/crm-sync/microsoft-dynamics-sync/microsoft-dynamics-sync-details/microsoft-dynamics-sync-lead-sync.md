---
unique-page-id: 3571848
description: Microsoft Dynamics Sync — 銷售機會同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 銷售機會同步
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft Dynamics同步：銷售機會同步 {#microsoft-dynamics-sync-lead-sync}

Marketo到Dynamics同步功能超強。 詳情如下：

## 如何使這兩個系統之間的詳細資訊保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

同步是雙向的。 如果您在Dynamics中變更銷售機會或在Marketo中變更人員，您的更新將會反映在兩個系統中。

>[!NOTE]
>
>刪除不一定會自動在兩個方向上同步。 請參閱 [刪除銷售機會或聯繫人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## 如果同時對兩個系統中的相同欄位進行變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這是罕見的，但Marketo將贏得人（領導），動力將贏得人脈。 這是因為我們認為營銷部門對人具有權威性，而官方的聯繫記錄系統是銷售(CRM)部門。

## 我可以使用Marketo在Dynamics中建立銷售機會嗎？ {#can-i-create-a-lead-in-dynamics-using-marketo}

是，請使用 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 流量動作。 如果銷售機會不存在，則會在Dynamics中建立銷售機會。 如果銷售機會確實存在，流程步驟將不執行任何操作。

>[!NOTE]
>
>使用「將人員同步至Microsoft」流量動作時（僅限於觸發促銷活動中），銷售機會/連絡人將在Dynamics中即時建立。

## 我可以手動將人員從Marketo強制同步至Dynamics中的銷售機會嗎？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

否，自動背景同步是在Marketo和Dynamics之間同步更新的唯一方式。 此 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 流操作不會強制銷售機會的同步。

## 哪些欄位會同步至Marketo? {#what-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) 進行設定。

## Marketo會遵守Dynamics驗證規則嗎？ {#will-marketo-respect-the-dynamics-validation-rules}

是。 如果資料格式錯誤或缺少必要欄位資訊，同步將會失敗。 如果發生此情況，Marketo會將結果記錄在人員的活動記錄中。
