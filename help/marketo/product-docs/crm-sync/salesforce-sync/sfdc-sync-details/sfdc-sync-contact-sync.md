---
unique-page-id: 2953457
description: SFDC同步——聯繫同步-Marketo文檔——產品文檔
title: SFDC同步——聯繫人同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# SFDC同步：連絡同步{#sfdc-sync-contact-sync}

您知道Marketo將您的整個資料庫與Salesforce同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何具體處理Salesforce Contacts的一些詳細資訊。

## 同步方向{#sync-direction}

聯繫人同步是雙向的。 如果您在Salesforce或Marketo變更連絡人，您的更新將反映在這兩個系統中。

## 如果同時在兩個系統中進行更改，該怎麼辦？{#what-if-changes-are-made-in-both-systems-at-the-same-time}

我們很好，讓Salesforce贏。 這種資料衝突很少發生。

## 我能將一個人變成Marketo的聯繫人嗎？{#can-i-convert-a-person-into-a-contact-in-marketo}

是，請使用&#x200B;**[轉換人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**&#x200B;流動動作。

>[!CAUTION]
>
>在Marketo轉換人員將會在Salesforce中產生新的帳戶和機會。 如果您不想要重複的帳戶，請使用Salesforce進行轉換。

## 我可以手動強制同步聯繫人嗎？{#can-i-manually-force-a-sync-of-a-contact}

是的，請使用「將人員同步到SFDC ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**流」操作，它將即時同步。**[

## 每個標準欄位都與Marketo同步嗎？{#does-every-single-standard-field-sync-to-marketo}

不，並非所有標準欄位都有用。 所有自訂欄位皆可成為同步的一部分。

>[!NOTE]
>
>Marketo將僅同步您的Marketo同步用戶有權訪問的欄位。

## Marketo會遵守Salesforce驗證規則嗎？{#will-marketo-respect-the-salesforce-validation-rules}

是的，如果發生衝突，則會將結果記錄在銷售線索活動日誌中。
