---
unique-page-id: 2953463
description: SFDC同步 — 銷售機會/帳戶擁有者同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 銷售機會/帳戶擁有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# SFDC同步：銷售機會/帳戶擁有者同步 {#sfdc-sync-lead-account-owner-sync}

技術上來說，這會同步Salesforce中的「使用者」表格，但我們會將其稱為銷售機會/帳戶擁有者欄位。

## 哪些欄位會同步至Marketo Engage？ {#which-fields-will-sync-to-marketo-engage}

對於同步至Marketo的每個人，我們也會同步以下擁有者欄位：

* 銷售擁有者名字
* 銷售負責人姓氏
* 銷售擁有者職稱
* 銷售負責人電話號碼
* 銷售負責人電子郵件地址

我們會為每個聯絡人同步上述五個潛在客戶擁有者欄位以及這些帳戶擁有者欄位：

* 帳戶擁有者名字
* 帳戶擁有者姓氏
* 帳戶擁有者電子郵件地址

## 我可以變更Marketo中的銷售機會擁有者嗎？ {#can-i-change-the-lead-owner-in-marketo}

絕對可以，只要使用 [變更擁有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"} 流量動作。

>[!NOTE]
>
>您無法使用變更擁有者資訊 [使用人員詳細資料頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## 我可以如何處理這些資料？ {#what-can-i-do-with-this-data}

使用此資料的原因很多，例如

* 傳送包含銷售擁有者簽名的個人化電子郵件
* 篩選特定銷售代表，以進行行銷或甚至分析成效
* Marketo中的指派（和重新指派）規則
* 在中使用它們 [變更擁有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Sync Person to SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}, and [Create Task](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程動作

Marketo的Salesforce同步處理確實非常棒。 沒有人能做得這麼好！
