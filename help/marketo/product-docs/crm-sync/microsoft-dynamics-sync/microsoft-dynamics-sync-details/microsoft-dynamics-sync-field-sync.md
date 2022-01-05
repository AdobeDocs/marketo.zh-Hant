---
unique-page-id: 3571838
description: Microsoft Dynamics Sync — 欄位同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 欄位同步
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics同步：欄位同步 {#microsoft-dynamics-sync-field-sync}

Marketo到Dynamics同步功能超強。 詳情如下。

## 兩個系統之間如何保持欄位詳細資訊的同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

對於Lead和Contact實體，同步是雙向的。 如果您在Dynamics中變更銷售機會或聯絡人，或在Marketo中變更人員，您的更新將會反映在兩個系統中。

對於帳戶、用戶、機會、團隊和自定義實體，同步是單向的：動態到Marketo。 如果您在Dynamics中變更這些實體，您的更新將會反映在Marketo中。

## 如果同時對兩個系統中的相同欄位進行變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這是罕見的，但Marketo將贏得人（領導），動力將贏得人脈。 這是因為我們認為營銷部門對人具有權威性，而官方的聯繫記錄系統是銷售(CRM)部門。 對於單向同步實體，Dynamics將始終勝出。

## 我可以使用Marketo在Dynamics中建立欄位嗎？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，目前不支援此功能。

## 我在Dynamics中建立了一個欄位。 我可以將它同步至Marketo嗎？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是的，你可以 [同步欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) 只要您的同步使用者在Dynamics中有權存取它，

## 哪些欄位會同步至Marketo? {#what-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) 進行設定。

## 如果在同步Marketo和Dynamics後需要新增自訂欄位，該怎麼辦？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以隨時新增欄位，並預期資料會從Dynamics重新整理至Marketo。 請參閱 [對新的自訂欄位使用與Microsoft Dynamics的快速同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) 以取得詳細資訊。

## 如果要在將欄位新增至同步後刪除Dynamics中的欄位，該怎麼辦？ {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [已禁用同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然後編輯並儲存Marketo中的結構，以重新整理 [選擇要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
