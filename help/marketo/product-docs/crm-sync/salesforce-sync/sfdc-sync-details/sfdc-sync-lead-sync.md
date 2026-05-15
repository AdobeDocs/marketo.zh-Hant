---
unique-page-id: 2953455
description: 瞭解銷售機會同步如何在Salesforce和Marketo之間運作。 瞭解雙向同步、從Marketo建立銷售機會，並遵守驗證規則。
title: SFDC同步 — 銷售機會同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/zqztwtX4Xe08Df-v1aTxhRi-cB2CZALctr3kaFNrT7s
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 2%

---

# SFDC 同步：商機同步 {#sfdc-sync-lead-sync}

從您的[!DNL Salesforce]資料庫同步Marketo。 它會同步、等待5分鐘，然後再次同步。 一整天，每天。 以下是Marketo如何特別處理[!DNL Salesforce]潛在客戶的一些詳細資料。

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

是的。 如果資料格式錯誤或遺失必要欄位資訊，同步處理將會失敗。 如果發生此情況，Marketo會將結果記錄在潛在客戶活動記錄中。
