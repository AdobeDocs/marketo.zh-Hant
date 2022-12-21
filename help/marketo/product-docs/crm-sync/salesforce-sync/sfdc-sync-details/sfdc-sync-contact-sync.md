---
unique-page-id: 2953457
description: SFDC同步 — 聯繫人同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 聯繫人同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# SFDC同步：聯繫人同步 {#sfdc-sync-contact-sync}

您是否知道Marketo會使用Salesforce同步您的整個資料庫？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是有關Marketo如何具體處理Salesforce連絡人的一些詳細資訊。

## 同步方向 {#sync-direction}

接觸同步是雙向的。 如果您在Salesforce或Marketo中變更連絡人，您的更新將會反映在這兩個系統中。

## 如果同時在兩個系統中進行變更，該怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我們很好，讓Salesforce贏。 這種資料衝突很少發生。

## 我可以在Marketo將人員轉換為聯絡人嗎？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，請使用 **[轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** 流量動作。

>[!CAUTION]
>
>在Marketo中轉換人員將在Salesforce中產生新帳戶和商機。 如果您不想要重複的帳戶，請使用Salesforce進行轉換。

## 我可以手動強制同步連絡人嗎？ {#can-i-manually-force-a-sync-of-a-contact}

是，請使用 **[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流程動作，且會即時同步。

## 每個標準欄位都會同步至Marketo嗎？ {#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自訂欄位都可以是同步的一部分。

>[!NOTE]
>
>Marketo只會同步您的Marketo同步使用者有權存取的欄位。

## Marketo是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

是，如果發生衝突，則會將結果記錄在銷售機會活動日誌中。
