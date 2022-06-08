---
unique-page-id: 2953463
description: SFDC同步 — 潛在客戶/客戶所有者同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 潛在客戶/帳戶所有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC同步：潛在客戶/帳戶所有者同步 {#sfdc-sync-lead-account-owner-sync}

這些表在技術上正在同步Salesforce中的「用戶」表，但我們將將其稱為「銷售線索/帳戶所有者」欄位。

## 哪些欄位將同步到Marketo? {#which-fields-will-sync-to-marketo}

對於同步到Marketo的每個人員，我們還同步以下所有者欄位：

* 銷售所有者名
* 銷售所有者姓
* 銷售所有者標題
* 銷售所有者電話號碼
* 銷售所有者電子郵件地址

對於每個聯繫人，我們將同步上述五個潛在客戶所有者欄位以及以下帳戶所有者欄位：

* 帳戶所有者名
* 帳戶所有者姓
* 帳戶所有者電子郵件地址

## 我能換下Marketo的主角嗎？ {#can-i-change-the-lead-owner-in-marketo}

當然，只要用 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) 流操作。

>[!NOTE]
>
>您不能使用 [使用「人員詳細資訊」頁](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)。

## 我可以利用這些資料做什麼？ {#what-can-i-do-with-this-data}

使用此資料有很多原因，例如

* 發送具有銷售所有者簽名的個性化電子郵件
* 篩選特定銷售代表以進行市場營銷甚至分析效果
* Marketo分配（和重新分配）規則
* 在 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)。 [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流動動作

Marketo的Salesforce同步功能真棒。 別人做得這麼好！
