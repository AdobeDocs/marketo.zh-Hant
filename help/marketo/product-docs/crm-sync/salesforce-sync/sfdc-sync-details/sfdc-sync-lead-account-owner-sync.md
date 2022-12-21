---
unique-page-id: 2953463
description: SFDC同步 — 銷售機會/客戶擁有者同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 銷售機會/帳戶所有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC同步：潛在客戶/帳戶擁有者同步 {#sfdc-sync-lead-account-owner-sync}

技術上，這些欄位正在同步Salesforce中的「使用者」表格，但我們將其稱為「銷售機會/帳戶擁有者」欄位。

## 哪些欄位會同步至Marketo? {#which-fields-will-sync-to-marketo}

對於同步至Marketo的每個人員，我們也同步下列擁有者欄位：

* 銷售負責人名字
* 銷售責任人姓氏
* 銷售所有者標題
* 銷售負責人電話號碼
* 銷售所有者電子郵件地址

對於每個聯繫人，我們同步了上述五個銷售機會所有者欄位以及以下帳戶所有者欄位：

* 帳戶擁有者名字
* 帳戶擁有者姓氏
* 帳戶擁有者電子郵件地址

## 我可以變更Marketo的銷售機會擁有者嗎？ {#can-i-change-the-lead-owner-in-marketo}

當然，只要使用 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) 流量動作。

>[!NOTE]
>
>您不能使用 [使用人員詳細資訊頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## 這些資料有什麼用？ {#what-can-i-do-with-this-data}

使用此資料的理由很多，例如

* 傳送具有銷售擁有者簽名的個人化電子郵件
* 篩選特定銷售代表以進行行銷或甚至分析成效
* Marketo的分配（和重新分配）規則
* 在 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)，和 [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流量動作

Marketo的Salesforce同步效果真不錯。 沒有人這麼做！
