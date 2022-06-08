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

您知道Marketo將整個資料庫與Salesforce同步嗎？ 它會同步，然後等待5分鐘，然後再次同步，一整天，每天。 下面是有關Marketo如何具體處理Salesforce聯繫人的一些詳細資訊。

## 同步方向 {#sync-direction}

聯繫人同步是雙向的。 如果您在Salesforce或Marketo中對聯繫人進行了更改，則您的更新將反映在兩個系統中。

## 如果同時在兩個系統中進行更改怎麼辦？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我們很好，讓Salesforce贏。 這種資料衝突很少發生。

## 我能把一個人變成Marketo的聯繫人嗎？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，使用 **[轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** 流操作。

>[!CAUTION]
>
>在Marketo轉換人員將在Salesforce中生成新帳戶和機會。 如果不想要重複的帳戶，請使用Salesforce進行轉換。

## 是否可以手動強制同步聯繫人？ {#can-i-manually-force-a-sync-of-a-contact}

是，使用 **[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流動操作，並即時同步。

## 每個標準欄位都與Marketo同步嗎？ {#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自定義欄位都可以是同步的一部分。

>[!NOTE]
>
>Marketo將僅同步您的Marketo同步用戶有權訪問的欄位。

## Marketo是否會遵守Salesforce驗證規則？ {#will-marketo-respect-the-salesforce-validation-rules}

是，如果存在衝突，則會將結果記錄在銷售線索活動日誌中。
