---
unique-page-id: 45417125
description: 針對非原生Salesforce整合的Sales Insight —— 行銷檔案——產品檔案
title: 針對非原生Salesforce整合的銷售分析
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 0%

---


# 非原生Salesforce整合的Sales Insight {#sales-insight-for-non-native-salesforce-integrations}

如果您的Marketo帳戶是透過自訂或非原生整合連線至Salesforce，請使用本檔案來設定Sales Insight。

>[!PREREQUISITES]
>
>* 在您開始設定MSI之前，為您的Marketo例項啟用「MSI非原生」功能標幟（如果未啟用，請連絡您的客戶成功經理）。
>* 設定[MSI套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)的Salesforce帳戶。
>* Marketo REST API [成功設定](https://developers.marketo.com/rest-api/)。 公開的CRUD API將是執行非原生同步的基礎。
>* 請閱讀[此部落格文章](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/)，以瞭解物件和關係。
>* 設定Salesforce物件，以顯示18個字元不區分大小寫的全域唯一識別碼，而非15個字元區分大小寫的全域唯一識別碼。


>[!NOTE]
>
>Marketo MSI管理面板中的REST API設定無法用於非原生同步。

## 成功執行MSI的非原生同步需要以下{#successful-non-native-sync-for-msi-requires-the-following}

1. 將Salesforce銷售使用者同步至Marketo。

   Salesforce Sales User是擁有Salesforce中Leads/Contacts的外部使用者。 需要為Salesforce Sales用戶更新行銷人員。 *externalSalesPersonId*&#x200B;欄位是負責Sales Person的新增。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo銷售人員欄位</strong></td> 
   <td><strong>Salesforce銷售使用者欄位</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales使用者不區分大小寫的全域唯一識別碼</td> 
   <td><p>將Marketo Sales Person記錄識別為外部Salesforce Sales User物件。</p><p>在同步其他物件之前，必須先同步銷售人員，以便建立正確的關係。</p></td> 
  </tr> 
 </tbody> 
</table>

銷售人員的API檔案：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
同步銷售人員的API檔案：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. 將Salesforce帳戶同步至Marketo。

   Salesforce帳戶需要升級Marketo Company。 _externalCompanyId_&#x200B;和&#x200B;_externalSalesPersonId_&#x200B;欄位是公司升級的授權欄位。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo公司欄位</strong></td> 
   <td><strong>Salesforce帳戶欄位</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帳戶不區分大小寫的全域唯一識別碼</td> 
   <td>識別外部Salesforce帳戶物件的Marketo Company記錄。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales使用者不區分大小寫的全域唯一識別碼</td> 
   <td>將Marketo Company記錄識別為帳戶擁有者的外部Salesforce Sales User物件。<br><br>亦用於Marketing，以將本公司與擁有本公司記錄之銷售人員建立關聯。在設定此欄位之前，必須先同步銷售人員。</td> 
  </tr> 
 </tbody> 
</table>

適用於公司的API檔案：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. 將Salesforce銷售線索／聯絡人同步至Marketo。

   您需要為Salesforce銷售線索／聯絡人插入Marketo Lead。 _externalPersonId_、_externalSalesPersonId_&#x200B;和&#x200B;_externalCompanyId_&#x200B;欄位是用於Lead的新增。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo銷售線索欄位</strong></td> 
   <td><strong>Salesforce銷售線索／聯繫人欄位</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforce銷售線索／連絡人不區分大小寫的全域唯一識別碼</td> 
   <td>將Marketo Lead記錄識別為外部Salesforce Lead/Contact物件。<br><br>這是為MSI非原生引入的新欄位。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales使用者不區分大小寫的全域唯一識別碼</td> 
   <td>識別擁有此Lead/Contact的外部Salesforce Sales User對象。<br><br>此外，銷售線索與Marketo中的銷售人員有關。要求首先正確同步銷售人員。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帳戶不區分大小寫的全域唯一識別碼</td> 
   <td>識別Lead/Contact所屬的外部Salesforce帳戶對象。<br><br>此外，銷售機會記錄也與Marketo中的一家公司有關。強制要求先正確同步Salesforce帳戶。</td> 
  </tr> 
 </tbody> 
</table>

銷售機會的API檔案：[`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
同步銷售機會的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 將Salesforce Opportunity與Marketo同步。

   您需要為Salesforce Opportunity插入Marketo Opportunity。 _externalOpportunityId_、_externalCompanyId_&#x200B;和&#x200B;_externalSalesPersonId_&#x200B;欄位是Opportunity的增補功能。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity對象欄位</strong></td> 
   <td><strong>Salesforce Opportunity物件欄位</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce銷售線索／連絡人不區分大小寫的全域唯一識別碼</td> 
   <td>將Marketo Opportunity記錄標識到外部Salesforce Opportunity對象。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帳戶不區分大小寫的全域唯一識別碼</td> 
   <td>標識此Opportunity所屬的外部Salesforce Account對象。 <br><br>強制要求先正確同步Salesforce帳戶。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales使用者不區分大小寫的全域唯一識別碼</td> 
   <td>標識擁有此Opportunity的外部Salesforce Sales User對象。 </td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文檔：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 將Salesforce連絡人角色同步至Marketo。

   然後，您可以透過Marketo Opportunity角色同步Salesforce Opportunity的Salesforce聯繫人角色。 Opportunity Role記錄要求&#x200B;_externalOpportunityId_ 、 _role_&#x200B;和&#x200B;_leadId_&#x200B;欄位。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity角色欄位</strong></td> 
   <td><strong>Salesforce連絡人角色欄位</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce Opportunity不區分大小寫的全域唯一識別碼</td> 
   <td>將Marketo Opportunity角色標識為外部Salesforce Opportunity對象。<br><br>Salesforce Opportunity必須先正確同步。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>N/A，此為Marketo Lead ID</td> 
   <td>這將是同步Salesforce連絡人的行銷人員銷售線索ID。<br><br>在Marketo中同步連絡人後，您可以使用Salesforce Contact不區分大小寫的全域唯一識別碼作為externalPersonId，並使用Marketo REST API查詢Marketo Lead。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td>Salesforce連絡人的角色欄位</td> 
   <td>說明此機會的聯繫人的角色。</td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文檔：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 將上一個有趣的時刻/MSI計分欄位同步至SFDC。

   在您的Salesforce物件正確同步至Marketo後，您就可以運用MSI功能。 MSI最後一個有趣的時刻／計分欄位將公開在REST API中，以取得銷售機會。 這些欄位是由MSI計算，且為唯讀。

   Marketo Lead的「最後一個有趣的時刻／計分」欄位必須使用REST API Lead端點定期同步至Salesforce。 使用&#x200B;_externalPersonId_&#x200B;作為filterType，並將Salesforce Lead GUID傳入為filterValue，查詢此端點的Marketo Lead。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   然後，您可以使用這些欄位的值，與Salesforce Lead/Contact物件同步。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo銷售線索欄位</strong></td> 
   <td><strong>Salesforce銷售線索／聯繫人欄位</strong></td> 
   <td><strong>說明</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentType</td> 
   <td>標籤：最後一個有趣的時刻類型<br>名稱：Last_Interect_Moment_Type_c</td> 
   <td>Lead的最後一個有趣時刻類型</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentDate</td> 
   <td><p>標籤：最後一個有趣的時刻</p><p>名稱：Last_Interect_Moment_Date_c</p></td> 
   <td>Lead的最後一個有趣時刻的日期</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentDesc</td> 
   <td><p>標籤：最後一個有趣的時刻說明</p><p>名稱：Last_Interect_Moment_Desc_c</p></td> 
   <td>Lead的最後一個有趣時刻說明</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentSource</td> 
   <td><p>標籤：最後一個有趣的時刻來源</p><p>名稱：Last_Interect_Moment_Source_c</p></td> 
   <td>Lead最後有趣時刻的來源</td> 
  </tr> 
  <tr> 
   <td>優先順序</td> 
   <td><p>標籤：參與</p><p>名稱：優先順序__c</p></td> 
   <td>Lead的優先順序</td> 
  </tr> 
  <tr> 
   <td>relativeUrgency</td> 
   <td><p>標籤：相對緊急值</p><p>名稱：緊急性_值_c</p></td> 
   <td>鉛的相對緊迫性</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>標籤：相對計分值</p><p>名稱：Relative_Score_Value_c</p></td> 
   <td>鉛的相對評分</td> 
  </tr> 
 </tbody> 
</table>

Lead REST API的檔案：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET)。

正確使用外部欄位是成功進行非原生同步的關鍵。 如果您在某些檢視中未看到資料，則可能會有特定欄位未正確同步。 例如，如果潛在客戶的活動和有趣的時刻在其帳戶下查看MSI介面工具集時未顯示，則潛在客戶的公司或帳戶可能未正確同步。 在指定外部欄位時執行此銷售機會的GET請求，將有助於您確認銷售機會是否正確同步。 此外，Marketing中外部銷售人員的電子郵件必須符合Salesforce中該使用者的電子郵件。 如果電子郵件不符，Salesforce的「行銷人員」索引標籤中可能不會顯示資料。
