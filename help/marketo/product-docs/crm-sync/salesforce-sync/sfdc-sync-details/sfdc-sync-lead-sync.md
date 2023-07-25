---
unique-page-id: 2953455
description: SFDC同步 — 銷售機會同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 潛在客戶同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC同步：潛在客戶同步 {#sfdc-sync-lead-sync}

您是否知道Salesforce資料庫中的Marketo同步？ 它會同步、等待5分鐘，然後再次同步。 一整天，每天。 以下詳細介紹Marketo如何特別對待Salesforce銷售機會。

## 同步方向 {#sync-direction}

銷售機會（人員）和連絡人同步是雙向的。 如果您在Salesforce或Marketo中變更記錄，您的更新將會反映在兩個系統中。

## 如果兩個系統同時進行變更，該怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo獲勝。 這類資料衝突很少發生。

## 我可以使用Marketo在Salesforce中建立銷售機會嗎？ {#can-i-create-a-lead-in-salesforce-using-marketo}

是，請使用 [將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流量動作。 如果銷售機會不存在，這會在Salesforce中建立銷售機會。

## 我可以手動強制將Marketo中的人員同步到Salesforce中的銷售機會嗎？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是，請使用 [將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流程動作，而且會即時同步。

## 每個標準欄位都會同步至Marketo嗎？ {#does-every-single-standard-field-sync-to-marketo}

否，並非所有標準欄位都有用。 所有自訂欄位都可以成為同步的一部分。

>[!NOTE]
>
>Marketo只會同步您的Salesforce同步使用者有權存取的欄位。

## Marketo是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

是. 如果資料格式錯誤或遺失必要欄位資訊，同步處理將會失敗。 如果發生此情況，Marketo會將結果記錄在潛在客戶活動記錄中。
