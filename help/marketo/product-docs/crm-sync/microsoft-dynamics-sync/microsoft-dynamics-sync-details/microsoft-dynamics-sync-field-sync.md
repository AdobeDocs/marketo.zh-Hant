---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync -Marketo文檔——產品文檔
title: Microsoft Dynamics Sync -Field Sync
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics Sync:欄位同步{#microsoft-dynamics-sync-field-sync}

Marketo到動態同步的功能非常強大。 以下是詳細資訊。

## 兩個系統之間如何保持欄位詳細資訊的同步？{#how-are-field-details-kept-in-sync-between-the-two-systems}

同步是引導實體和連絡實體的雙向同步。 如果您在Dynamics或Marketo地區變更銷售線索或連絡人，您的更新將反映在這兩個系統中。

對於帳戶、用戶、機會、團隊和自定義實體，同步是單向的：Marketo。 如果您在Dynamics中變更這些實體，您的更新會反映在Marketo。

## 如果同時對兩個系統中的同一欄位進行更改，該怎麼辦？ （資料衝突）{#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將贏得人（領導），動力將贏得人脈。 這是因為我們認為行銷部門對人有權威性，而官方的聯絡記錄系統則位於銷售(CRM)部門。 對於單向同步實體，Dynamics將永遠勝出。

## 我是否可使用Marketo在Dynamics中建立欄位？{#can-i-create-a-field-in-dynamics-using-marketo}

否，目前不支援此功能。

## 我在動力學(Dynamics)上建立了一個欄位。 我能把它同步到Marketo嗎？{#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是的，只要您的同步使用者在Dynamics中有存取權，您就可以[同步欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)。

## 哪些欄位會與Marketo同步？{#what-fields-will-sync-to-marketo}

您可以在設定期間選取要同步的欄位。[](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)

## 如果我需要在Marketo和動態同步後新增自訂欄位，該怎麼辦？{#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以隨時新增欄位，並期待資料從Dynamics重新整理至Marketo。 如需詳細資訊，請參閱[使用與Microsoft Dynamics快速同步以取得新自訂欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)。

## 如果我想在將欄位新增至同步後刪除Dynamics中的欄位，該怎麼辦？{#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo儲存要同步的欄位參考。 如果您刪除Dynamics中的欄位，我們建議您在[sync disabled](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)下執行此動作。 然後，通過編輯和保存[選擇要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)來刷新Marketo的模式。
