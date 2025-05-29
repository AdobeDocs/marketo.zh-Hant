---
solution: Marketo Engage
product: marketo
title: Personalization Token
description: 瞭解如何在新的Marketo Engage電子郵件Designer中使用個人化代號
level: Beginner, Intermediate
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
source-git-commit: c31f338d7f784258a120c90a9d5016366d5a1095
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Personalization Token {#personalization-tokens}

在電子郵件個人化Token方面，電子郵件設計工具的格式與傳統電子郵件編輯器不同。 已實作此變更的目的是改善與Handlebar指令碼的相容性，並簡化您的電子郵件建立流程。

>[!AVAILABILITY]
>
>自2025年5月23日起，此功能將批次布建給Marketo Engage使用者，每週會更新一個區域。 轉出期間，使用新電子郵件設計工具建立的任何電子郵件都會自動將現有Token移轉到新格式。 透過此更新，所有Token都將僅提供英文版。

## 主要使用案例 {#primary-use-case}

此增強功能主要有利於從[Velocity指令碼](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/email-scripting){target="_blank"}轉換成Handlebar指令碼的使用者。 新的電子郵件設計工具僅支援新的權杖格式。 更新後的格式消除了空格，並引進了修訂後的預設文字結構，以確保更順暢且更有效的指令碼體驗。

## 權杖體驗 {#token-experience}

檢視權杖體驗，包括舊體驗和新體驗。

### 舊格式 {#old-format}

在傳統電子郵件編輯器中，您可以新增含空格的權杖，例如`lead.Anonymous IP`或`member.registration code`。 預設文字的格式為： `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="500" zoomable="yes"}

### 新格式 {#new-format}

在電子郵件設計工具中，您必須使用[駝峰式大小寫](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case)或標籤底線（例如`lead.anonymousIP`或`member.registration_code`）。 預設文字的格式也會變更為`{%=lead.city ?: "fallback" %}`。

![](assets/personalization-tokens-2.png){width="600" zoomable="yes"}

## 注意事項 {#things-to-note}

* 為了方便編寫，個人化編輯器也提供下列功能：

   * 還原/重做
   * 尋找/尋找和取代
   * 自動完成

* 新的個人化編輯器支援Marketo Engage先前支援的&#x200B;**所有**&#x200B;權杖。
