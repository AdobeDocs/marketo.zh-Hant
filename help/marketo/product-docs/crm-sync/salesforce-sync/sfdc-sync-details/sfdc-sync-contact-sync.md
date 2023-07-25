---
unique-page-id: 2953457
description: SFDC同步 — 連絡人同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 連絡人同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# SFDC同步：連絡人同步 {#sfdc-sync-contact-sync}

您知道Marketo會將您的整個資料庫與Salesforce同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別對待Salesforce聯絡人的部分細節。

## 同步方向 {#sync-direction}

連絡人同步是雙向的。 如果您在Salesforce或Marketo中變更連絡人，您的更新將會反映在這兩個系統中。

## 如果兩個系統同時進行變更，該怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我們很好，讓Salesforce獲勝。 這類資料衝突很少發生。

## 我可以在Marketo中將個人轉換為聯絡人嗎？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，請使用 **[轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** 流量動作。

>[!CAUTION]
>
>在Marketo中轉換人員將在Salesforce中產生新帳戶和機會。 如果您不想要重複的帳戶，請使用Salesforce進行轉換。

## 我可以手動強制同步處理連絡人嗎？ {#can-i-manually-force-a-sync-of-a-contact}

是，請使用 **[將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流程動作，而且會即時同步。

## 每個標準欄位都會同步至Marketo嗎？ {#does-every-single-standard-field-sync-to-marketo}

否，並非所有標準欄位都有用。 所有自訂欄位都可以成為同步的一部分。

>[!NOTE]
>
>Marketo只會同步您的Marketo同步使用者有權存取的欄位。

## Marketo是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

是，如果發生衝突，則會將結果記錄在潛在客戶活動記錄中。
