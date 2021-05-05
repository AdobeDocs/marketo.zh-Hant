---
unique-page-id: 2950799
description: 預付碼概述-Marketo文檔——產品文檔
title: 預付碼概觀
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
translation-type: tm+mt
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 預付碼概述{#tokens-overview}

Token是可用於Marketo智慧型促銷活動流程步驟、電子郵件、登陸頁面、程式碼片段和網頁促銷活動的變數。

## 瞭解預設值{#understanding-default-values}

當您使用Token時，您也想要提供預設值。 此文字會顯示人員是否沒有您所參照欄位的值。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此範例中，電子郵件會顯示「Greetings,（名字）」或「Greetings, earthling」（預設值）。

![](assets/two.png)

>[!CAUTION]
>
>使用Marketo的電子郵件編輯器時，代號無法在前標中運作。 若要在前標中使用Token，它必須透過您在電子郵件範本中的HTML。

>[!NOTE]
>
>這份清單並非完整無遺。 您也會針對您在Marketo的每個自訂欄位建立Token。

## 人員代號{#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* 如果您使用自訂人員欄位的顯示名稱，例如`{{lead.Custom Field Name}}`，自訂人員欄位也能運作

## 公司預付碼{#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* 如果您使用自訂公司欄位的顯示名稱（例如），自訂公司欄位也能運作。`{{Company.Custom Field Name}}`

## 促銷活動Token {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系統Token {#system-tokens}

>[!NOTE]
>
>在[系統代號辭彙表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)中進一步瞭解這些代號。

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## 觸發Token {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>根據智慧型促銷活動中使用的觸發器，尋找[標籤的詳細資訊，以瞭解有趣的時刻](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)。

## 程式Token {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## 我的代號{#my-tokens}

我的Token是在程式中定義的，開頭為`{{my.`，後面是您為Token建立的名稱。 進一步瞭解[程式中的My Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)。

## 成員Token {#member-token}

會員代號可用來插入整合服務合作夥伴的唯一值。 會員代號的常見用途是讓網路研討會與會者使用獨特的URL。 每個人都有一個唯一URL，可存取網路研討會，並可使用`{{member.webinar url}}`代號來插入。 `{{member.webinar url}}`代號會自動解析服務提供者產生的個人唯一確認URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>`{{member.webinar url}}` Token僅會在傳送電子郵件的智慧型促銷活動是事件程式的子資產時填入。
