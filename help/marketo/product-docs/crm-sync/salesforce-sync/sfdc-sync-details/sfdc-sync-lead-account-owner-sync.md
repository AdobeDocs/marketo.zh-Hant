---
unique-page-id: 2953463
description: SFDC同步——銷售線索／客戶擁有者同步-Marketo文檔——產品文檔
title: SFDC同步——銷售線索／帳戶擁有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC同步：銷售線索／帳戶擁有者同步{#sfdc-sync-lead-account-owner-sync}

這些表格在技術上正在同步Salesforce中的「使用者」表格，不過我們會將其稱為「銷售機會／帳戶擁有者」欄位。

## 哪些欄位會與Marketo同步？{#which-fields-will-sync-to-marketo}

對於同步至Marketo的每個人，我們也會同步下列擁有者欄位：

* 銷售擁有者名字
* 銷售擁有者姓氏
* 銷售擁有者標題
* 銷售人員電話號碼
* 銷售擁有者電子郵件地址

對於每個聯繫人，我們同步上述五個銷售線索責任人欄位以及這些帳戶責任人欄位：

* 帳戶擁有者名字
* 帳戶擁有者姓氏
* 帳戶擁有者電子郵件地址

## 我能換掉Marketo的主銷嗎？{#can-i-change-the-lead-owner-in-marketo}

當然，只要使用[Change Owner](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)流動操作即可。

>[!NOTE]
>
>您不能使用[使用人員詳細資訊頁](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)更改所有者資訊。

## 我可以如何處理這些資料？{#what-can-i-do-with-this-data}

有許多理由可使用此資料，例如

* 從銷售擁有者傳送具有簽名的個人化電子郵件
* 篩選特定銷售代表以進行行銷或甚至分析成效
* Marketo分配（和重新分配）規則
* 在[更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)、[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)和[建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)流操作中使用它們

Marketo的Salesforce同步功能絕佳。 沒有人能這麼做！
