---
unique-page-id: 2953455
description: SFDC同步——銷售線索同步——行銷人員文檔——產品文檔
title: SFDC同步——銷售線索同步
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# SFDC同步：銷售線索同步{#sfdc-sync-lead-sync}

您知道Marketo會從您的Salesforce資料庫同步嗎？ 它會同步，等待5分鐘，然後再次同步。 整天，每天。 以下是Marketo如何特別對待Salesforce銷售機會的一些詳細資訊。

## 同步方向{#sync-direction}

潛在客戶（人）和連絡人同步是雙向的。 如果您在Salesforce或Marketo中變更記錄，您的更新將會反映在這兩種系統中。

## 如果同時在兩個系統中進行更改，該怎麼辦？{#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo贏。 這種資料衝突很少發生。

## 我是否可以使用Marketo在Salesforce中建立銷售機會？{#can-i-create-a-lead-in-salesforce-using-marketo}

是的，請使用[將人員同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流操作。 如果銷售線索不存在，這會在Salesforce中建立銷售線索。

## 我是否可手動強制Marketing中的人員同步至Salesforce中的銷售線索？{#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是的，請使用「將人員同步到SFDC[流」操作，它將即時同步。](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)

## 每個標準欄位是否都與Marketo同步？{#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自訂欄位皆可成為同步的一部分。

>[!NOTE]
>
>Marketo只會同步您的Salesforce同步使用者可存取的欄位。

## Market是否會遵守Salesforce驗證規則？{#will-marketo-respect-the-salesforce-validation-rules}

是的。 如果資料格式錯誤或遺失必要欄位資訊，同步將會失敗。 Marketo會將此結果記錄在銷售機會活動記錄中（如果發生此情況）。
