---
unique-page-id: 2953455
description: SFDC Sync — 銷售機會同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 潛在客戶同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# SFDC同步：潛在客戶同步 {#sfdc-sync-lead-sync}

您是否知道Salesforce資料庫中的Marketo Engage同步？ 它會同步、等待5分鐘，然後再次同步。 一整天，每天。 以下是Marketo如何特別對待Salesforce潛在客戶的一些細節。

## 同步方向 {#sync-direction}

銷售機會（人員）和連絡人同步是雙向的。 如果您在Salesforce或Marketo中變更記錄，您的更新將會反映在兩個系統中。

## 如果兩個系統同時進行變更，該怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo獲勝。 很少發生這類資料衝突。

## 我可以使用Marketo在Salesforce中建立銷售機會嗎？ {#can-i-create-a-lead-in-salesforce-using-marketo}

是，請使用 [將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} 流量動作。 如果銷售機會不存在，這會在Salesforce中建立銷售機會。

## 我可以手動強制同步處理Marketo中的人員至Salesforce中的銷售機會嗎？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是，請使用 [將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} 流程動作，而且會即時同步。

## 每個標準欄位都會同步至Marketo嗎？ {#does-every-single-standard-field-sync-to-marketo}

否，並非所有標準欄位都有用。 所有自訂欄位都可成為同步處理的一部分。

>[!NOTE]
>
>Marketo將只會同步您的Salesforce同步使用者有權存取的欄位。

## Marketo是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

有。如果資料格式錯誤或遺失必要欄位資訊，同步處理將會失敗。 如果發生此情況，Marketo會將結果記錄在潛在客戶活動記錄中。
