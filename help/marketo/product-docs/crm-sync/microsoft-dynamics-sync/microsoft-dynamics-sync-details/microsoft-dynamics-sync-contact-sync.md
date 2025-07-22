---
unique-page-id: 3571833
description: Microsoft Dynamics同步 — 連絡人同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 連絡人同步
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步處理：連絡人同步處理 {#microsoft-dynamics-sync-contact-sync}

您知道Marketo會將您的整個資料庫與[!DNL Dynamics]同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別處理[!DNL Dynamics]聯絡人的部分細節。

## 兩個系統之間的詳細資料如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

連絡人同步是雙向的。 如果您變更[!DNL Dynamics]中的連絡人或Marketo中的人員，您的更新將會反映在這兩個系統中。

## 如果兩個系統中的相同欄位同時發生變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將贏得人心，而[!DNL Dynamics]將贏得連絡人。 這是因為我們認為行銷部門是人員的權威，而聯絡人的官方記錄系統是在銷售(CRM)部門。

## 我可以使用Marketo建立連絡人嗎？ {#can-i-create-a-contact-using-marketo}

可以。[以下是](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}的方式。

>[!NOTE]
>
>使用「將人員同步至Microsoft」流程動作時（僅限觸發器行銷活動中），將在[!DNL Dynamics]中即時建立銷售機會/聯絡人。

## 我可以手動強制同步處理人員或連絡人嗎？ {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

否，自動背景同步是Marketo與[!DNL Dynamics]之間同步更新的唯一方法。 [將人員同步至Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)不會強制同步處理潛在客戶。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可在安裝期間[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)。 但Marketo將只會同步您的[!DNL Dynamics]同步使用者有權存取的欄位。

## Marketo是否會遵守[!DNL Dynamics]驗證規則？ {#will-marketo-respect-the-dynamics-validation-rules}

是，如果發生衝突，則會將結果記錄在潛在客戶活動記錄中。
