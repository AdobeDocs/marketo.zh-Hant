---
unique-page-id: 1147344
description: 系統權杖字彙表 — Marketo檔案 — 產品檔案
title: 系統權杖字彙表
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 系統權杖字彙表 {#system-tokens-glossary}

除了人員代號之外，您也可以使用一些特別酷的系統代號。 這些區段在這裡。

>[!NOTE]
>
>您的帳戶時區設定會影響日期和時間Token的執行時間。

## system.date {#system-date}

此 `{{system.date}}` Token會在執行階段轉譯目前日期，如下所示： **2013年8月08日**

**運作方式：**

* [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} 流程步驟
* [有趣的時刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} 流程步驟
* [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程步驟
* 電子郵件或範本的正文

## system.time {#system-time}

此 `{{system.time}}` Token會在執行階段轉譯目前時間，如下所示： **下午04:34 (GMT -0700)**

**運作方式：**

* [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} 流程步驟
* [有趣的時刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} 流程步驟
* [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程步驟
* 電子郵件或範本的正文

## system.dateTime {#system-datetime}

此 `{{system.dateTime}}` Token會在執行階段呈現目前的日期和時間，如下所示： **2013-08-08 16:36:13**

**運作方式：**

* [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} 流程步驟
* [有趣的時刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} 流程步驟
* [建立任務](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程步驟
* 電子郵件或範本的正文

## system.forwardToFriendLink {#system-forwardtofriendlink}

此 `{{system.forwardToFriendLink}}` 代號可讓您控制 [電子郵件中的「轉寄給朋友連結」](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**運作方式：**

* [新增系統權杖作為電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} 或範本

## system.unsubscribeLink {#system-unsubscribelink}

此 `{{system.unsubscribeLink}}` 代號可讓您控制電子郵件中取消訂閱連結的位置。

**運作方式：**

* [新增系統權杖作為電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} 或範本

## system.viewAsWebpageLink {#system-viewaswebpagelink}

此 `{{system.viewAsWebpageLink}}` 代號可讓您控制電子郵件中「以網頁形式檢視」連結的位置。

**搭配使用：**

* [新增系統權杖作為電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} 或範本
