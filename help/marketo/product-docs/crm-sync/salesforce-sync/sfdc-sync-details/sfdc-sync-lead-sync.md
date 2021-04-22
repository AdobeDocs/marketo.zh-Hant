---
unique-page-id: 2953455
description: SFDC同步——銷售線索同步-Marketo文檔——產品文檔
title: SFDC同步——銷售線索同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC同步：銷售線索同步{#sfdc-sync-lead-sync}

您知道Salesforce資料庫中的Marketo同步嗎？ 它會同步，等待5分鐘，然後再次同步。 整天，每天。 以下是有關Marketo如何具體對待Salesforce銷售機會的一些詳細資訊。

## 同步方向{#sync-direction}

潛在客戶（人）和連絡人同步是雙向的。 如果您在Salesforce或Marketo中變更記錄，您的更新將會反映在這兩種系統中。

## 如果同時在兩個系統中進行更改，該怎麼辦？{#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo贏了。 這種資料衝突很少發生。

## 我是否可以使用Marketo在Salesforce中建立銷售機會？{#can-i-create-a-lead-in-salesforce-using-marketo}

是的，請使用[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流操作。 如果銷售線索不存在，這會在Salesforce中建立銷售線索。

## 我是否可以手動強制Marketo的人員同步至Salesforce的銷售線索？{#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是的，請使用「將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流」操作，它將即時同步。[

## 每個標準欄位都與Marketo同步嗎？{#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自訂欄位皆可成為同步的一部分。

>[!NOTE]
>
>Marketo將只同步您的Salesforce同步使用者可存取的欄位。

## Marketo會遵守Salesforce驗證規則嗎？{#will-marketo-respect-the-salesforce-validation-rules}

是的。 如果資料格式錯誤或遺失必要欄位資訊，同步將會失敗。 Marketo將在銷售線索活動日誌中記錄結果（如果發生這種情況）。
