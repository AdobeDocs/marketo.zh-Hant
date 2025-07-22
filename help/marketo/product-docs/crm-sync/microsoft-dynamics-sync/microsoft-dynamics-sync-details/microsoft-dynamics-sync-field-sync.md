---
unique-page-id: 3571838
description: Microsoft Dynamics同步 — 欄位同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 欄位同步
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步：欄位同步 {#microsoft-dynamics-sync-field-sync}

Marketo與[!DNL Dynamics]的同步處理功能非常強大。 詳情如下。

## 兩個系統之間的欄位詳細資料如何保持同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

潛在客戶與聯絡人實體的同步是雙向的。 如果您在[!DNL Dynamics]中變更銷售機會或連絡人，或在Marketo中變更人員，您的更新將會反映在這兩個系統中。

對於帳戶、使用者、商機、團隊和自訂實體，同步是單向的： [!DNL Dynamics]到Marketo。 如果您在[!DNL Dynamics]中變更這些實體，您的更新將會反映在Marketo中。

## 如果兩個系統中的相同欄位同時發生變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將會贏得人員（潛在客戶），而[!DNL Dynamics]將會贏得連絡人。 這是因為我們認為行銷部門是人員的權威，而聯絡人的官方記錄系統是在銷售(CRM)部門。 對於單向同步實體，[!DNL Dynamics]將一律獲勝。

## 我可以使用Marketo在[!DNL Dynamics]中建立欄位嗎？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，目前不支援此功能。

## 我在[!DNL Dynamics]中建立了一個欄位。 我可以將其同步至Marketo嗎？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

可以，只要您的同步使用者在[中擁有欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)的存取權，您就可以[!DNL Dynamics]同步欄位。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可在安裝期間[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。

## 如果我需要在同步Marketo和[!DNL Dynamics]後新增自訂欄位，該怎麼辦？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以隨時新增欄位，並期待資料從[!DNL Dynamics]重新整理到Marketo。 如需詳細資訊，請參閱[新自訂欄位的 [!DNL Microsoft Dynamics] 使用快速同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)。

## 如果要在欄位新增至同步後刪除[!DNL Dynamics]中的欄位，該怎麼辦？ {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo會儲存要同步之欄位的參考。 如果您刪除[!DNL Dynamics]中的欄位，我們建議您在停用[同步處理](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情況下進行刪除。 接著，編輯並儲存[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)，以重新整理Marketo中的結構描述。
