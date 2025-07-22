---
description: 預設動態欄位對應 — Marketo檔案 — 產品檔案
title: 預設動態欄位對應
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# 預設動態欄位對應 {#default-dynamics-field-mapping}

當您初次將Marketo Engage帳戶與Microsoft同步時，Marketo會自動在內建的Dynamics和Marketo欄位之間建立這些關聯。  Marketo也會同步處理潛在客戶、帳戶、商機和聯絡人上的自訂欄位。

## 潛在客戶欄位 {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo欄位</th>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>[!UICONTROL Created On]</td>
      <td>建立</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL First Name]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL Middle Name]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last]</td>
      <td>[!UICONTROL Last Name]</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>電子郵件地址1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Job Title]</td>
      <td>[!UICONTROL Job title]</td>
      <td>工作標題</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>電話1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobile Phone]</td>
      <td>行動電話</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fax]</td>
      <td>[!UICONTROL Fax]</td>
      <td>傳真</td>
    </tr>
    <tr>
      <td>[!UICONTROL Address]</td>
      <td>[!UICONTROL Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL City]</td>
      <td>[!UICONTROL City]</td>
      <td>地址1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL State]</td>
      <td>[!UICONTROL State/Province]</td>
      <td>address1_stateorprovidle</td>
    </tr>
    <tr>
      <td>[!UICONTROL Country]</td>
      <td>[!UICONTROL Country/Region]</td>
      <td>address1country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postal Code]</td>
      <td>[!UICONTROL Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Source]</td>
      <td>[!UICONTROL Lead Source]</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>狀態代碼</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>說明</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do Not Call]</td>
      <td>[!UICONTROL Do Not Allow Phone Calls]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Unsubscribed]</td>
      <td>[!UICONTROL Do not bulk email]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Rating]</td>
      <td>[!UICONTROL Rating]</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 2]</td>
      <td>[!UICONTROL Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 3]</td>
      <td>[!UICONTROL Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Email]</td>
      <td>[!UICONTROL Do Not Allow Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Do Not Allow Faxes]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Send Marketing Material]</td>
      <td>[!UICONTROL Marketing Material]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Home Phone]</td>
      <td>電話2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Preferred Method Of Contact]</td>
      <td>[!UICONTROL Preferred Method of Contact]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Topic]</td>
      <td>[!UICONTROL Topic]</td>
      <td>主旨</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Company Name]</td>
      <td>companyname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Score]</td>
      <td>[!UICONTROL Relative Score]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Priority]</td>
      <td>[!UICONTROL Priority]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgency]</td>
      <td>mkt_urgency</td>
    </tr>
    <tr>
      <td>[!UICONTROL Subject]</td>
      <td>[!UICONTROL Topic]</td>
      <td>主旨</td>
    </tr>
    <tr>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>收入</td>
    </tr>
  </tbody>
</table>

以下Lead欄位會同步以供內部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>建立</td>
    </tr>
  </tbody>
</table>

## 連絡人欄位 {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo欄位</th>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>[!UICONTROL Created On]</td>
      <td>建立</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL First Name]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL Middle Name]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last]</td>
      <td>[!UICONTROL Last Name]</td>
      <td>姓氏</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>電子郵件地址1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Job Title]</td>
      <td>[!UICONTROL Job Title]</td>
      <td>工作標題</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>電話1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobile Phone]</td>
      <td>行動電話</td>
    </tr>
    <tr>
      <td>[!UICONTROL Address]</td>
      <td>[!UICONTROL Address 1: Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL City]</td>
      <td>[!UICONTROL Address 1: City]</td>
      <td>地址1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL State]</td>
      <td>[!UICONTROL Address 1: State/Province]</td>
      <td>address1_stateorprovidle</td>
    </tr>
    <tr>
      <td>[!UICONTROL Country]</td>
      <td>[!UICONTROL Address 1: Country/Region]</td>
      <td>address1country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postal Code]</td>
      <td>[!UICONTROL Address 1: Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>狀態代碼</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do Not Call]</td>
      <td>[!UICONTROL Do Not Allow Phone Calls]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Unsubscribed]</td>
      <td>[!UICONTROL Do not bulk email]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 2]</td>
      <td>[!UICONTROL Address 1: Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 3]</td>
      <td>[!UICONTROL Address 1: Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Email]</td>
      <td>[!UICONTROL Do Not Allow Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Home Phone]</td>
      <td>電話2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Preferred Method Of Contact]</td>
      <td>[!UICONTROL Preferred Method Of Contact]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Send Marketing Material]</td>
      <td>[!UICONTROL Marketing Material]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Priority]</td>
      <td>[!UICONTROL Priority]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgency]</td>
      <td>mkt_urgency</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Score]</td>
      <td>[!UICONTROL Relative Score]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>說明 </td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Score]</td>
      <td>[!UICONTROL Lead Score]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>說明 </td>
    </tr>
  </tbody>
</table>

以下連絡人欄位會同步以供內部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>建立</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company Name]</td>
      <td>parentcustomerid</td>
    </tr>
  </tbody>
</table>

## 帳戶欄位 {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo欄位</th>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Account (a)]</td>
      <td>[!UICONTROL Account]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Address]</td>
      <td>[!UICONTROL Address 1: Street 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing City]</td>
      <td>[!UICONTROL Address 1: City]</td>
      <td>地址1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Country]</td>
      <td>[!UICONTROL Address 1: Country/Region]</td>
      <td>address1country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Postal Code]</td>
      <td>[!UICONTROL Address 1: Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Billing Address 2]</td>
      <td>[!UICONTROL Address 1: Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Billing Address 3]</td>
      <td>[!UICONTROL Address 1: Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Main Phone]</td>
      <td>[!UICONTROL Main Phone]</td>
      <td>電話1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Business Type]</td>
      <td>[!UICONTROL Business Type]</td>
      <td>businesstypecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Account Number]</td>
      <td>[!UICONTROL Account Number]</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Company Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>收入</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>說明</td>
    </tr>
    <tr>
      <td>[!UICONTROL Industry]</td>
      <td>[!UICONTROL Industry]</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC Code]</td>
      <td>[!UICONTROL SIC Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Website]</td>
      <td>[!UICONTROL Website]</td>
      <td>網站</td>
    </tr>
    <tr>
      <td>[!UICONTROL Num Employees]</td>
      <td>[!UICONTROL Number of Employees]</td>
      <td>number女性</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC Code]</td>
      <td>[!UICONTROL SIC Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Account Name]</td>
      <td>名稱</td>
    </tr>
    <tr>
      <td>[!UICONTROL Num Employees]</td>
      <td>[!UICONTROL Number of Employees]</td>
      <td>number女性</td>
    </tr>
  </tbody>
</table>

以下帳戶欄位會同步以供內部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>建立</td>
    </tr>
  </tbody>
</table>

## 機會欄位 {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo欄位</th>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Close Probability]</td>
      <td>[!UICONTROL Probabliity]</td>
      <td>closeprobability</td>
    </tr>
    <tr>
      <td>[!UICONTROL Stage]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Actual Close Date]</td>
      <td>[!UICONTROL Actual Close Date]</td>
      <td>actualclosedate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Name]</td>
      <td>[!UICONTROL Topic]</td>
      <td>名稱</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estimated Value]</td>
      <td>[!UICONTROL Est. Revenue]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL Description]</td>
      <td>[!UICONTROL Description]</td>
      <td>說明</td>
    </tr>
  </tbody>
</table>

以下帳戶欄位會同步以供內部使用。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics欄位</th>
      <th>MS Dynamics API名稱</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Opportunity]</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL Potential Customer]</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Marketo中Microsoft相關的系統欄位（唯讀） {#microsoft-related-system-fields}

以下欄位是在Marketo中建立的，但使用者無法調整。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo欄位</th>
      <th>說明</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Type]</td>
      <td>潛在客戶或連絡人。 如果空白，該潛在客戶在Marketo中只會以個人身分存在</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>在[!DNL MS Dynamics]中建立的日期(可能與Marketo中的建立日期不同)</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft is Deleted]</td>
      <td>此人之前在Microsoft但遭到刪除，現在僅居住在Marketo</td>
    </tr>
  </tbody>
</table>
