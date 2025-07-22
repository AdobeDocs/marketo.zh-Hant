---
unique-page-id: 3571848
description: Microsoft Dynamics同步 — 銷售機會同步 — Marketo檔案 — 產品檔案
title: Microsoft Dynamics同步 — 銷售機會同步
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步：潛在客戶同步 {#microsoft-dynamics-sync-lead-sync}

Marketo與[!DNL Dynamics]的同步處理功能非常強大。 詳細資料如下：

## 兩個系統之間的詳細資料如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

同步是雙向的。 如果您變更[!DNL Dynamics]中的潛在客戶或Marketo中的人員，您的更新將會反映在兩個系統中。

>[!NOTE]
>
>刪除並不總是自動雙向同步。 請參閱[刪除銷售機會或連絡人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}。

## 如果兩個系統中的相同欄位同時發生變更，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將會贏得人員（潛在客戶），而[!DNL Dynamics]將會贏得連絡人。 這是因為我們認為行銷部門是人員的權威，而聯絡人的官方記錄系統是在銷售(CRM)部門。

## 我可以使用Marketo在[!DNL Dynamics]中建立銷售機會嗎？ {#can-i-create-a-lead-in-dynamics-using-marketo}

是，使用[[!UICONTROL Sync Person to Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流程動作。 如果潛在客戶不存在，這會在[!DNL Dynamics]中建立潛在客戶。 如果潛在客戶確實存在，則流程步驟將不會執行任何動作。

>[!NOTE]
>
>使用&quot;[!UICONTROL Sync Person to Microsoft]&quot;流量動作時（僅限觸發促銷活動），將在[!DNL Dynamics]中即時建立銷售機會/聯絡人。

## 我可以手動強制將人員從Marketo同步處理至[!DNL Dynamics]中的銷售機會嗎？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

否，自動背景同步是Marketo與[!DNL Dynamics]之間同步更新的唯一方法。 [[!UICONTROL Sync Person to Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流程動作不會強制同步處理潛在客戶。

## 哪些欄位會同步至Marketo？ {#what-fields-will-sync-to-marketo}

您可在安裝期間[選取要同步處理的欄位](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。

## Marketo是否會遵守[!DNL Dynamics]驗證規則？ {#will-marketo-respect-the-dynamics-validation-rules}

可以。如果資料格式錯誤或遺失必要欄位資訊，同步處理將會失敗。 如果發生此情況，Marketo會將結果記錄在人員的活動記錄中。
