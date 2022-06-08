---
unique-page-id: 2953455
description: SFDC同步 — Lead Sync -Marketo文檔 — 產品文檔
title: SFDC同步 — 潛在客戶同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC同步：潛在客戶同步 {#sfdc-sync-lead-sync}

您知道Marketo從Salesforce資料庫中同步嗎？ 它同步，等待5分鐘，然後再次同步。 一整天，每天。 下面是有關Marketo如何具體處理Salesforce銷售線索的一些詳細資訊。

## 同步方向 {#sync-direction}

線索（人）和聯繫人同步是雙向的。 如果您對Salesforce或Marketo中的記錄進行了更改，則更新將反映在兩個系統中。

## 如果同時在兩個系統中進行更改怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo贏了。 這種資料衝突很少發生。

## 我能否使用Marketo在Salesforce中建立銷售線索？ {#can-i-create-a-lead-in-salesforce-using-marketo}

是，使用 [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流操作。 如果Salesforce中不存在潛在顧客，這將建立潛在顧客。

## 我是否可以手動強制Marketo人員的同步到Salesforce的主管？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是，使用 [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流動操作，並即時同步。

## 每個標準欄位都與Marketo同步嗎？ {#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自定義欄位都可以是同步的一部分。

>[!NOTE]
>
>Marketo將僅同步您的Salesforce同步用戶有權訪問的欄位。

## Marketo是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

是. 如果資料格式錯誤或缺少必需欄位資訊，同步將失敗。 如果發生這種情況，Marketo將將結果記錄在lead活動日誌中。
