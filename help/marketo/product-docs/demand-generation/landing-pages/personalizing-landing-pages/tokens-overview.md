---
unique-page-id: 2950799
description: Token概述 — Marketo檔案 — 產品檔案
title: Token概述
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Token概述 {#tokens-overview}

代號是可用於Marketo智慧行銷活動流程步驟、電子郵件、登入頁面、代碼片段和網頁行銷活動的變數。

## 瞭解預設值 {#understanding-default-values}

使用Token時，您也要提供預設值。 這是顯示某人是否沒有您所參考欄位值的文字。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此範例中，電子郵件會顯示「Greetings， （名字）」或「Greetings， earthling」（預設值）。

![](assets/two.png)

>[!CAUTION]
>
>使用Marketo的電子郵件編輯器時，Token無法在預覽版中運作。 若要在預覽文字中使用Token，必須透過電子郵件範本中您自己的HTML進行。

>[!NOTE]
>
>此清單並非詳盡無遺。 系統也會為您在Marketo中擁有的每個自訂欄位建立代號。

## 人員Token {#person-tokens}

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
* 如果您使用其顯示名稱，例如， `{{lead.Custom Field Name}}`

## 公司Token {#company-tokens}

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
* 如果您使用其顯示名稱，自訂公司欄位也可運作，例如： `{{Company.Custom Field Name}}`

## 行銷活動Token {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系統Token {#system-tokens}

>[!NOTE]
>
>若要深入瞭解這些Token，請參閱 [系統權杖字彙表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

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
>尋找更多關於以下內容的詳細資訊： [有趣時刻的代號](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) 根據智慧行銷活動中使用的觸發程式。

## 計畫代號 {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## 我的Token {#my-tokens}

我的Token是在方案中定義的，且開頭為 `{{my.` 後面接著您為權杖建立的名稱。 進一步瞭解 [方案中的我的Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## 成員權杖 {#member-token}

成員Token可用來插入整合式服務合作夥伴的唯一值。 「成員代號」的常見用途是網路研討會出席者的唯一URL。 每個人都有唯一URL可存取可使用插入的網路研討會 `{{member.webinar url}}` token。 此 `{{member.webinar url}}` 代號會自動解析服務提供者產生的個人唯一確認URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>此 `{{member.webinar url}}` 只有當傳送電子郵件的智慧型行銷活動是事件計畫的子資產時，才會填入Token。
