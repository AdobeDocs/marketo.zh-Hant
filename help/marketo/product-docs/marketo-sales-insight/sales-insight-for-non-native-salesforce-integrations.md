---
unique-page-id: 45417125
description: 針對非本地Salesforce整合的Sales Insight -Marketo文檔 — 產品文檔
title: 針對非本地Salesforce整合的Sales Insight
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: fb663ddf4c0021f258317636fbc7794e8172ab7e
workflow-type: tm+mt
source-wordcount: '1400'
ht-degree: 0%

---

# 針對非本地Salesforce整合的Sales Insight {#sales-insight-for-non-native-salesforce-integrations}

如果您的Adobe Marketo Engage帳戶通過自定義或非本機整合連接到Salesforce，請使用本文配置Sales Insight。

>[!PREREQUISITES]
>
>* 在開始設定MSI之前，為您的Marketo實例啟用的「MSI非本機」功能(如果未啟用，並且您已購買該功能，請聯繫 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} — 如果您尚未購買此功能，請與客戶成功經理聯繫)。
>* Salesforce帳戶 [MSI包設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}。
>* MarketoREST API [已成功設定](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}。 外露的CRUD API將是執行非本機同步的基礎。
>* 閱讀 [此部落格帖子](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;}，以便瞭解對象和關係。
>* 設定Salesforce對象以顯示18個字元的不區分大小寫全局唯一標識符，而不是15個字元的區分大小寫全局唯一標識符。


>[!NOTE]
>
>MarketoMSI管理面板中的REST API配置不能用於非本機同步。

## 成功執行MSI的非本機同步需要以下 {#successful-non-native-sync-for-msi-requires-the-following}

1. 將Salesforce Sales用戶同步到Marketo。

   Salesforce Sales User是擁有Salesforce中Leads/Contact的外部用戶。 需要為Salesforce Sales用戶更新Marketo銷售人員。 的 *外部SalesPersonId* 欄位是用於Sales Person的更新的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo銷售人員欄位</strong></td> 
      <td><strong>Salesforce Sales用戶欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td><p>標識外部Salesforce Sales User對象的MarketoSales Person記錄。</p><p>它要求在同步其他對象之前先同步銷售人員，以便建立正確的關係。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售人員的API文檔： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;
   * 用於同步銷售人員的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target=&quot;_blank&quot;

1. 將Salesforce帳戶同步到Marketo。

   需要為Salesforce帳戶更新Marketo公司。 的 _外部公司ID_ 和 _外部SalesPersonId_ 欄位的授權範圍。

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
      <td>外部公司ID</td> 
      <td>Salesforce帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識外部Salesforce帳戶對象的Marketo公司記錄。</td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識作為帳戶所有者的外部Salesforce Sales User對象的Marketo公司記錄。<br><br>亦用於Marketo內，將本公司與擁有本公司記錄之銷售人士聯繫。 必須先同步銷售人員，然後才能設定此欄位。</td> 
     </tr> 
    </tbody> 
   </table>

   * 公司API文檔： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;
   * 用於同步公司的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Companys/syncCompanysingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companys/syncCompanysingPOST){target=&quot;_blank&quot;

1. 將Salesforce Leads/Contacts同步到Marketo。

   您需要為Salesforce Lead/Contact添加一個MarketoLead。 的 _外部人員ID_。 _外部SalesPersonId_, _外部公司ID_ 欄位是用於Lead的上插的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo領隊</strong></td> 
      <td><strong>Salesforce Lead/Contact欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部人員ID</td> 
      <td>Salesforce Lead/Contact全局唯一標識符不區分大小寫</td> 
      <td>標識外部Salesforce Lead/Contact對象的MarketoLead記錄。<br><br>這是為MSI非本機引入的新欄位。</td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識擁有此Lead/Contact的外部Salesforce Sales User對象。<br><br>還將銷售線索與Marketo的銷售人員聯繫起來。 要求首先讓銷售人員正確同步。</td> 
     </tr> 
     <tr> 
      <td>外部公司ID</td> 
      <td>Salesforce帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識Lead/Contact所屬的外部Salesforce帳戶對象。<br><br>還將領先記錄與Marketo的一家公司有關。 要求首先正確同步Salesforce帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售線索的API文檔： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * 用於同步銷售線索的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 將Salesforce Opportunities同步到Marketo。

   您需要為Salesforce Opportunity添加一個MarketoOpportunity。 的 _外部機會ID_。 _外部公司ID_, _外部SalesPersonId_ 欄位是為Opportunity的upsert指定的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會對象欄位</strong></td> 
      <td><strong>Salesforce Opportunity對象欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部機會ID</td> 
      <td>Salesforce Lead/Contact全局唯一標識符不區分大小寫</td> 
      <td>標識外部Salesforce Opportunity對象的MarketoOpportunity記錄。</td> 
     </tr> 
     <tr> 
      <td>外部公司ID</td> 
      <td>Salesforce帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識此Opportunity所屬的外部Salesforce帳戶對象。 <br><br>要求首先正確同步Salesforce帳戶。</td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識擁有此Opportunity的外部Salesforce Sales User對象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;
   * 用於同步Opportunity的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Opportunity/syncOpportunityUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportunityUsingPOST){target=&quot;_blank&quot;

1. 將Salesforce聯繫人角色同步到Marketo。

   然後，可以通過MarketoOpportunity角色同步Salesforce Opportunity的Salesforce Contact角色。 Opportunity Role記錄要求 _外部機會ID_。 _角色_, _leadId_ 的子菜單。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會角色欄位</strong></td> 
      <td><strong>Salesforce聯繫人角色欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部機會ID</td> 
      <td>Salesforce Opportunity不區分大小寫的全局唯一標識符</td> 
      <td>標識外部Salesforce Opportunity對象的MarketoOpportunity角色。<br><br>要求首先正確同步Salesforce Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/A，這是Marketo線索ID</td> 
      <td>這將是同步的Salesforce聯繫人的Marketo線索ID。<br><br>聯繫人在Marketo同步後，您可以使用Salesforce Contact不區分大小寫的全局唯一標識符作為externalPersonId，並使用MarketoREST API查詢MarketoLead。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>Salesforce聯繫人的「角色」欄位</td> 
      <td>描述此機會的聯繫人角色。</td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;
   * 用於同步Opportunity的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Opportunity/syncOpportunityUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportunityUsingPOST){target=&quot;_blank&quot;

1. 將「上次感興趣的時刻/MSI計分」欄位同步到SFDC。

   Salesforce對象正確同步到Marketo後，您就可以利用MSI功能。 MSI「最後感興趣的時刻/評分」欄位將在REST API中為Lead顯示。 這些欄位由MSI計算，且為只讀欄位。

   MarketoLead的「最後一個有趣的時刻/評分」欄位需要使用REST API Lead終結點定期同步到Salesforce。 使用 _外部人員ID_ 作為filterType，並將Salesforce Lead GUID作為filterValue傳遞。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   然後，您可以使用這些欄位的值與Salesforce Lead/Contact對象同步。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo領隊</strong></td> 
      <td><strong>Salesforce Lead/Contact欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterectMomentType</td> 
      <td>標籤：最後有趣的時刻類型<br>名稱：Last_Interent_Moment_Type_c</td> 
      <td>Lead的最後有趣時刻的類型</td> 
     </tr> 
     <tr> 
      <td>msiLastInteretMomentDate</td> 
      <td><p>標籤：最後有趣的時刻日期</p><p>名稱：Last_Interent_Moment_Date_c</p></td> 
      <td>Lead的最後一個有趣時刻的日期</td> 
     </tr> 
     <tr> 
      <td>msiLastInterectMomentDesc</td> 
      <td><p>標籤：最後一個有趣的時刻說明</p><p>名稱：Last_Interent_Moment_Desc_c</p></td> 
      <td>Lead最後一個有趣時刻的說明</td> 
     </tr> 
     <tr> 
      <td>msiLastInteredMomentSource</td> 
      <td><p>標籤：最後有趣的時刻源</p><p>名稱：Last_Interent_Moment_Source_c</p></td> 
      <td>線索最後有趣時刻的來源</td> 
     </tr> 
     <tr> 
      <td>優先順序</td> 
      <td><p>標籤：參與</p><p>名稱：優先順序__c</p></td> 
      <td>Lead的優先順序</td> 
     </tr> 
     <tr> 
      <td>相對緊急性</td> 
      <td><p>標籤：相對緊急度值</p><p>名稱：緊急性_值_c</p></td> 
      <td>Lead的相對緊急性</td> 
     </tr> 
     <tr> 
      <td>相對計分</td> 
      <td><p>標籤：相對計分值</p><p>名稱：相對分數值</p></td> 
      <td>Lead的相對評分</td> 
     </tr> 
    </tbody> 
   </table>

   Lead REST API的文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}。

   正確使用外部欄位是成功進行非本機同步的關鍵。 如果在某些視圖中未能看到資料，則可能某個欄位未正確同步。 例如，如果潛在客戶在其帳戶下查看MSI構件時未顯示潛在客戶的活動和有趣時刻，則潛在客戶的公司或帳戶可能未正確同步。 在指定外部欄位時執行此潛在顧客的GET請求將幫助您驗證潛在顧客是否正確同步。 此外，Marketo外部銷售人員的電子郵件必須與Salesforce中該用戶的電子郵件相匹配。 如果電子郵件不匹配，則資料可能不會顯示在Salesforce的「Marketo」頁籤中。
