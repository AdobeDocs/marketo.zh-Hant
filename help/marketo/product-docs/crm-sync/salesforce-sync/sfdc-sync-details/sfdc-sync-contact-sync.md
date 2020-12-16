---
unique-page-id: 2953457
description: SFDC同步——聯絡同步——行銷文檔——產品文檔
title: SFDC同步——聯繫人同步
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# SFDC同步：連絡人同步 {#sfdc-sync-contact-sync}

您知道Market會將整個資料庫與Salesforce同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何具體處理Salesforce連絡人的詳細資訊。

## 同步方向 {#sync-direction}

聯繫人同步是雙向的。 如果您在Salesforce或Marketo中變更連絡人，您的更新將會反映在這兩個系統中。

## 如果同時在兩個系統中進行更改，該怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我們很好，讓Salesforce贏。 這種資料衝突很少發生。

## 我是否可將人員轉換為Marketo中的聯絡人？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是的，請使用** [Convert Person](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**流程動作。

>[!CAUTION]
>
>將Marketing中的人員轉換為Salesforce中的人員，將產生新帳戶和商機。 如果您不想要重複的帳戶，請使用Salesforce進行轉換。

## 我可以手動強制同步聯繫人嗎？ {#can-i-manually-force-a-sync-of-a-contact}

是的，請使用** [Sync Person to SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **flow操作，它將即時同步。

## 每個標準欄位是否都與Marketo同步？ {#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自訂欄位皆可成為同步的一部分。

>[!NOTE]
>
>Marketo只會同步您的Marketo同步使用者可存取的欄位。

## Market是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

是的，如果發生衝突，則會將結果記錄在銷售線索活動日誌中。
