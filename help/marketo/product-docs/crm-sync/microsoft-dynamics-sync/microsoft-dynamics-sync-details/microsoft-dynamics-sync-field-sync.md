---
unique-page-id: 3571838
description: Microsoft Dynamics同步 — 欄位同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 欄位同步
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics同步：欄位同步 {#microsoft-dynamics-sync-field-sync}

Marketo與Dynamics同步處理功能非常強大。 詳情如下。

## 兩個系統之間的欄位詳細資料如何保持同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

潛在客戶與連絡人實體的同步是雙向的。 如果您變更Dynamics中的銷售機會或連絡人，或Marketo中的人員，您的更新將會反映在這兩個系統中。

對於帳戶、使用者、商機、團隊和自訂實體，同步是單向的：Dynamics至Marketo。 如果您在Dynamics中變更這些實體，您的更新將會反映在Marketo中。

## 如果兩個系統中的相同欄位同時發生變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將會贏得人員（銷售機會），而Dynamics將會贏得連絡人。 這是因為我們認為行銷部門是人員的權威，而聯絡人的官方記錄系統是在銷售(CRM)部門。 對於單向同步實體，Dynamics將一律獲勝。

## 我可以使用Marketo在Dynamics中建立欄位嗎？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，目前不支援此功能。

## 我在Dynamics中建立了一個欄位。 我可以將其同步至Marketo嗎？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是，您可以 [同步欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 只要您的同步處理使用者能在Dynamics中存取。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可以 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 於設定期間。

## 如果我需要在同步Marketo和Dynamics後新增自訂欄位，該怎麼辦？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以隨時新增欄位，並預期資料會從Dynamics重新整理至Marketo。 另請參閱 [使用與Microsoft Dynamics快速同步處理新自訂欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) 以取得詳細資訊。

## 將欄位新增至同步後，如果我想刪除Dynamics中的欄位，該怎麼辦？ {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo會儲存要同步之欄位的參考。 如果您刪除Dynamics中的欄位，建議您使用 [同步已停用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然後編輯並儲存，重新整理Marketo中的結構描述 [選取要同步的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
