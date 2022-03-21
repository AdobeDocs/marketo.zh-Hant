---
description: 為什麼我的動態欄位未填寫 — Marketo文檔 — 產品文檔
title: 為什麼我的動態欄位不填
hide: true
hidefromtoc: true
source-git-commit: 8e31c2da9351d784e97d3d2bfe0d3d07dfab8961
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 為什麼我的動態欄位不填 {#why-arent-my-dynamic-fields-filling-out}

只有在使用模板時，動態欄位才會工作。 你撰寫的個別一次性電子郵件不會填寫這些內容。

## 檢查內容 {#what-to-check}

Sales Insight Actions中有三種類型的動態欄位：基本、自定義和Salesforce。 基本和自定義都可從 [Web應用](https://toutapp.com/login)。 如果Web應用程式中不存在該資訊，則欄位將為空。 Salesforce欄位從中提取資訊 [Salesforce.com](https://salesforce.com)。

**疑難解答Salesforce欄位**

Salesforce欄位：例如 `{{sfdc_account_name}}`

* 確保它與Sales Insight Actions正確連接。 轉到 [設定](https://toutapp.com/login) 的 **管理** 在CRM旁邊。

**基本欄位和自定義欄位疑難解答**

輸出基本欄位：例如 `{{company}}`

輸出自定義欄位：例如 `{{custom_field_favorite_movie}}`

* 需要為您的聯繫人保存相應欄位 [人物頁](https://toutapp.com/next#relationships) 供動態領域參考。 例如，如果您向Mary發送電子郵件， `{{company}}` 但是她的聯繫記錄沒有列出公司，我們將無法填寫。

## 為什麼在不填充所有動態欄位的情況下發送電子郵件？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果無法填充電子郵件中的所有動態欄位， Sales Insight Actions將阻止您發送電子郵件。 **但是**，此規則有幾個例外。 某些欄位將發送為空，或自動填充值（如果可以找到）。 下面列出了這些欄位，以及如果它們無法填充該欄位，將作何反應。

`{{first_name}}` =空

`{{last_name}}` =空

`{{title}}` =空

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>的 `{{first_name}}` 欄位將在Sales Insight Actions和Salesforce中查找以嘗試獲取資訊。 此清單中的所有其他欄位僅在Sales Insight Actions中查找以填充該欄位。
