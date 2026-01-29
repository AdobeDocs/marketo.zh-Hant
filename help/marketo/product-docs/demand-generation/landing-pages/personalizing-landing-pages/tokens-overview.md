---
unique-page-id: 2950799
description: 權杖概觀 - Marketo 文件 - 產品文件
title: 權杖概觀
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '296'
ht-degree: 100%

---

# 權杖概觀 {#tokens-overview}

權杖是可用於 Marketo 智慧行銷活動流程步驟、電子郵件、登陸頁面、程式碼片段和網頁行銷活動的變數。

## 了解預設值 {#understanding-default-values}

使用權杖時，您也要提供預設值。如果某個人員在您所參照的欄位中沒有任何值，就會顯示這段文字。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此範例中，電子郵件會顯示「(first name)，您好」或「earthling，您好」(預設值)。

![](assets/two.png)

>[!CAUTION]
>
>使用 Marketo 的電子郵件編輯器時，權杖無法在預覽文字中運作。若要在預覽文字中使用權杖，您必須透過電子郵件範本中您自己的 HTML 進行。

>[!NOTE]
>
>此清單並非完整清單。系統也會針對您在 Marketo 中擁有的每個自訂欄位建立權杖。

## 人員權杖 {#person-tokens}

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
* 如果您使用自訂人員欄位的顯示名稱，則也同樣可正常運作，例如 `{{lead.Custom Field Name}}`。

## 公司權杖 {#company-tokens}

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
* 如果您使用自訂公司欄位的顯示名稱，則也同樣可正常運作，例如：`{{Company.Custom Field Name}}`

## 行銷活動權杖 {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系統權杖 {#system-tokens}

>[!NOTE]
>
>若要了解更多有關這些權杖的資訊，請參閱[系統權杖字彙表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)。

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## 觸發程序權杖 {#trigger-tokens}

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
>根據在智慧行銷活動中所使用的觸發程序，尋找更多有關[關鍵時刻的權杖](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)的詳細資料。

## 方案權杖 {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL My Tokens] {#my-tokens}

[!UICONTROL My Tokens]是在方案中進行定義，且以 `{{my.` 開頭，後接您為權杖所建立的名稱。了解更多有關[「方案中的我的權杖」](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)的資訊。

## 成員權杖 {#member-token}

成員權杖可用於插入整合式服務合作夥伴的唯一值。成員權杖的常見用途為網路研討會出席者的唯一 URL。每個使用者都有唯一 URL，可用於存取可使用 `{{member.webinar url}}` 權杖插入的網路研討會。`{{member.webinar url}}` 權杖會自動解析服務提供者所產生的個人唯一確認 URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>只有在傳送電子郵件的智慧行銷活動為事件方案的下層資產時，`{{member.webinar url}}` 權杖才會填入。
