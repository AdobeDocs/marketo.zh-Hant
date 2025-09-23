---
unique-page-id: 2953455
description: SFDC同步 — 銷售機會同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 銷售機會同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 2%

---

# SFDC 同步：商機同步 {#sfdc-sync-lead-sync}

您知道來自[!DNL Salesforce]資料庫的Marketo同步嗎？ 它會同步、等待5分鐘，然後再次同步。 一整天，每天。 以下是Marketo如何特別處理[!DNL Salesforce]潛在客戶的一些詳細資料。

## 同步方向 {#sync-direction}

銷售機會（人員）和連絡人同步是雙向的。 如果您在[!DNL Salesforce]或Marketo中變更記錄，您的更新將會反映在兩個系統中。

## 如果兩個系統同時進行變更，該怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo獲勝。 很少發生這類資料衝突。

## 我可以使用Marketo在[!DNL Salesforce]中建立銷售機會嗎？ {#can-i-create-a-lead-in-salesforce-using-marketo}

是，使用[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流程動作。 如果潛在客戶不存在，這會在[!DNL Salesforce]中建立潛在客戶。

## 我可以手動強制將Marketo中的人員同步處理至[!DNL Salesforce]中的銷售機會嗎？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是，使用[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}流程動作，它將會即時同步。

## 每個標準欄位都會同步至Marketo嗎？ {#does-every-single-standard-field-sync-to-marketo}

否，並非所有標準欄位都有用。 所有自訂欄位都可成為同步處理的一部分。

>[!NOTE]
>
>Marketo將只會同步您的[!DNL Salesforce]同步使用者有權存取的欄位。

## Marketo是否會遵守[!DNL Salesforce]驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

可以。如果資料格式錯誤或遺失必要欄位資訊，同步處理將會失敗。 如果發生此情況，Marketo會將結果記錄在潛在客戶活動記錄中。
