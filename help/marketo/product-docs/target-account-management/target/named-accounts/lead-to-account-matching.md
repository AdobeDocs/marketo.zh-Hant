---
unique-page-id: 11381156
description: 銷售機會與帳戶匹配——行銷人員檔案——產品檔案
title: 銷售機會與帳戶匹配
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 導致帳戶匹配{#lead-to-account-matching}

使用Marketo Lead-to-Account比對，將右側銷售機會比對至正確的已命名帳戶。

>[!NOTE]
>
>**銷售線索至帳戶** 匹配是Marketo Target帳戶管理的內建功能。它採用模糊邏輯，幾乎即時地自動匹配指定帳戶的潛在客戶。 這些指名的帳戶可以是CRM帳戶或Marketo公司。

Marketo Lead-to-Account匹配遵循4個步驟流程：

**步驟1 —— 我** 們的匹配流程從使用銷售線索記錄的關鍵資訊開始，例如：

* 電子郵件網域（例如acme.com）
* 從IP位址推斷出公司名稱
* 公司名稱——這可以是CRM帳戶名稱或潛在客戶公司名稱屬性（例如，來自表單填寫）

**步驟2 —— 我** 們根據各種銷售機會屬性來標準化我們尋找的公司名稱（例如，Acme Inc.和Acme Corp會自動標準化為Acme）。此步驟可確保我們在Marketo中擁有指名帳戶的單一表示法，並可在單一指名帳戶中查看所有潛在客戶。

**步驟3 —— 我** 們將匹配的銷售機會分成2個桶：強比和弱比。

* 弱匹配銷售機會出現在已命名的帳戶上，然後可以手動解決。

**步驟4 —— 我** 們列出了一份具有強項和弱項的擬議公司清單。當根據其中一家建議的公司建立指名帳戶時，我們會建立符合規則，以自動將新的銷售機會（例如，銷售機會填寫表單）關聯至正確的指名帳戶。 這樣，您就不必再擔心匹配銷售機會，而更擔心獲得收入！

由於Marketo Lead-to-Account比對是Marketo Target帳戶管理的內建功能，因此比對Lead會以近乎即時的方式發生（例如，當銷售機會填寫Marketto表單時，我們會將所述銷售機會關聯至正確的命名帳戶）。 此事件可用來觸發警報，並通知帳戶擁有者新銷售機會來自其指定帳戶。

>[!NOTE]
>
>如果您在Salesforce中使用LeanData進行「銷售線索至帳戶」比對，Marketo的整合會將這些比對同步至您的Marketo例項。 若要啟用該功能，請聯絡[行銷支援](https://nation.marketo.com/t5/Support/ct-p/Support)。

>[!MORELIKETHIS]
>
>[Discover帳戶](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
