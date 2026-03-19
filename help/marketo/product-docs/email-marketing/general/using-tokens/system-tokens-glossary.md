---
unique-page-id: 1147344
description: 瞭解Marketo電子郵件中可用的系統權杖。 使用字彙表尋找適合個人化的代號。
title: 系統權杖字彙表
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 2%

---

# 系統權杖字彙表 {#system-tokens-glossary}

除了人員代號之外，您也可以使用一些特別酷的系統代號。 這些區段在這裡。

>[!NOTE]
>
>您的帳戶時區設定會影響日期和時間Token的執行時間。

## system.date {#system-date}

`{{system.date}}`權杖將在執行階段呈現目前日期，如下所示： **Aug 08， 2013**

**工作位置：**

* [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}流程步驟
* [有趣的時刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}流程步驟
* [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}流程步驟
* 電子郵件或範本的正文

## system.time {#system-time}

`{{system.time}}`權杖將在執行階段呈現目前時間，例如： **04:34下午(GMT -0700)**

**工作位置：**

* [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}流程步驟
* [有趣的時刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}流程步驟
* [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}流程步驟
* 電子郵件或範本的正文

## system.dateTime {#system-datetime}

`{{system.dateTime}}`權杖將在執行階段呈現目前的日期和時間，如下所示： **2013-08-08 16:36:13**

**工作位置：**

* [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}流程步驟
* [有趣的時刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}流程步驟
* [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}流程步驟
* 電子郵件或範本的正文

## system.unsubscribeLink {#system-unsubscribelink}

`{{system.unsubscribeLink}}` Token可讓您控制電子郵件中取消訂閱連結的位置。

**工作位置：**

* [新增系統權杖作為電子郵件或範本中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}

## system.viewAsWebpageLink {#system-viewaswebpagelink}

`{{system.viewAsWebpageLink}}` Token可讓您控制電子郵件中「以網頁形式檢視」連結的位置。

**使用：**

* [新增系統權杖作為電子郵件或範本中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}
