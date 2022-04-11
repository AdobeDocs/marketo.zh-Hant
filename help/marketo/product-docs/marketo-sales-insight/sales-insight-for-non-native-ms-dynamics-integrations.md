---
description: 針對非本機MS Dynamics整合的Sales Insight -Marketo文檔 — 產品文檔
title: 針對非本機MS Dynamics整合的Sales Insight
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
source-git-commit: ff076d66a193664aa6ec05cf940143cebdd2d942
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 針對非本機MS Dynamics整合的Sales Insight {#sales-insight-for-non-native-ms-dynamics-integrations}

如果您的Adobe Marketo Engage帳戶通過自定義或非本機整合連接到MS Dynamics，請使用本文配置Sales Insight。

>[!PREREQUISITES]
>
>* 在開始設定MSI之前，為您的Marketo實例啟用的「MSI非本機」功能(如果未啟用，並且您已購買該功能，請聯繫 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} — 如果您尚未購買此功能，請與客戶成功經理聯繫)。
>* 下載 [用於自定義同步的MSI包](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}。
>* MS Dynamics訂閱，帶MSI安裝程式([按預先](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-365.md){target=&quot;_blank&quot;, [Dynamics聯機](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target=&quot;_blank&quot;})。
>* MarketoREST API [已成功設定](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}。 外露的CRUD API將是執行非本機同步的基礎。
>* 閱讀 [此部落格帖子](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;}，以便瞭解對象和關係。


## 成功執行MSI的非本機同步需要以下 {#successful-non-native-sync-for-msi-requires-the-following}

1. 將MS Dynamics Sales用戶同步到Marketo。

   MS Dynamics Sales User是MS Dynamics中擁有Lead/Contacts的外部用戶。 需要為MS Dynamics Sales用戶更新Marketo銷售人員。 外部SalesPersonId欄位是為Sales Person的更新指定的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo銷售人員欄位</strong></td> 
      <td><strong>MS Dynamics用戶欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>MS Dynamics用戶不區分大小寫全局唯一標識符</td> 
      <td><p>標識外部MS Dynamics User對象的Marketo銷售人員記錄。</p><p>它要求在同步其他對象之前先同步銷售人員，以便建立正確的關係。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售人員的API文檔： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;
   * 用於同步銷售人員的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target=&quot;_blank&quot;

1. 將MS Dynamics帳戶同步到Marketo。

   Marketo公司需要為MS Dynamics帳戶更新。 的 _外部公司ID_ 和 _外部SalesPersonId_ 欄位的授權範圍。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo公司欄位</strong></td> 
      <td><strong>MS Dynamics帳戶欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部公司ID</td> 
      <td>MS Dynamics帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識外部MS Dynamics帳戶對象的Marketo公司記錄。</td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>MS Dynamics Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>將Marketo公司記錄標識為外部MS Dynamics Sales User對象（該對象是帳戶所有者）。<br><br>亦用於Marketo內，將本公司與擁有本公司記錄之銷售人士聯繫。 必須先同步銷售人員，然後才能設定此欄位。</td> 
     </tr> 
    </tbody> 
   </table>

   * 公司API文檔： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;
   * 用於同步公司的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Companys/syncCompanysingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companys/syncCompanysingPOST){target=&quot;_blank&quot;

1. 將MS Dynamics Leads/Contacts同步到Marketo。

   您需要為MS Dynamics Lead/Contact插入一個MarketoLead。 的 _外部人員ID_。 _外部SalesPersonId_, _外部公司ID_ 欄位是用於Lead的上插的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo領隊</strong></td> 
      <td><strong>MS Dynamics線索/聯繫人欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部人員ID</td> 
      <td>MS Dynamics Lead/Contact全局唯一標識符不區分大小寫</td> 
      <td>標識外部MS Dynamics Lead/Contact對象的MarketoLead記錄。<br><br>這是為MSI非本機引入的新欄位。</td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>MS Dynamics Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識擁有此Lead/Contact的外部MS Dynamics Sales User對象。<br><br>還將銷售線索與Marketo的銷售人員聯繫起來。 要求首先讓銷售人員正確同步。</td> 
     </tr> 
     <tr> 
      <td>外部公司ID</td> 
      <td>MS Dynamics帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識Lead/Contact所屬的外部MS Dynamics帳戶對象。<br><br>還將領先記錄與Marketo的一家公司有關。 要求先正確同步MS Dynamics帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售線索的API文檔： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target=&quot;_blank&quot;
   * 用於同步銷售線索的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target=&quot;_blank&quot;

1. 將MS Dynamics Opportunities同步到Marketo。

   您需要為MS Dynamics Opportunity添加Marketo機會。 的 _外部機會ID_。 _外部公司ID_, _外部SalesPersonId_ 欄位是為Opportunity的upsert指定的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會對象欄位</strong></td> 
      <td><strong>MS Dynamics Opportunity對象欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部機會ID</td> 
      <td>MS Dynamics Lead/Contact全局唯一標識符不區分大小寫</td> 
      <td>標識外部MS Dynamics Opportunity對象的MarketoOpportunity記錄。</td> 
     </tr> 
     <tr> 
      <td>外部公司ID</td> 
      <td>MS Dynamics帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識此Opportunity所屬的外部MS Dynamics Account對象。 <br><br>要求先正確同步MS Dynamics帳戶。</td> 
     </tr> 
     <tr> 
      <td>外部SalesPersonId</td> 
      <td>MS Dynamics Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識擁有此Opportunity的外部MS Dynamics Sales User對象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;
   * 用於同步Opportunity的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Opportunity/syncOpportunityUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportunityUsingPOST){target=&quot;_blank&quot;

1. 將MS Dynamics聯繫人角色同步到Marketo。

   然後，可以通過MarketoOpportunity Role同步MS Dynamics Opportunity的MS Dynamics Contact Roles。 Opportunity Role記錄要求 _外部機會ID_。 _角色_, _leadId_ 的子菜單。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會角色欄位</strong></td> 
      <td><strong>MS Dynamics聯繫人角色欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>外部機會ID</td> 
      <td>MS Dynamics Opportunity全局唯一標識符不區分大小寫</td> 
      <td>標識外部MS Dynamics Opportunity對象的MarketoOpportunity角色。<br><br>要求先正確同步MS Dynamics Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/A，這是Marketo線索ID</td> 
      <td>這將是同步的MS Dynamics Contact的Marketo線索ID。<br><br>聯繫人在Marketo同步後，您可以使用MS Dynamics Contact全局不區分大小寫的唯一標識符作為外部PersonId，並使用MarketoREST API查詢Marketo線索。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>MS Dynamics Contact的「角色」欄位</td> 
      <td>描述此機會的聯繫人角色。</td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;
   * 用於同步Opportunity的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Opportunity/syncOpportunityUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportunityUsingPOST){target=&quot;_blank&quot;

1. 將「上次感興趣的時刻/MSI計分」欄位同步到MS Dynamics。

   MS Dynamics對象正確同步到Marketo後，您就可以利用MSI功能。 MSI「最後感興趣的時刻/評分」欄位將在REST API中為Lead顯示。 這些欄位由MSI計算，且為只讀欄位。

   需要使用REST API Lead終結點將MarketoLead的「最後感興趣的時刻/評分」欄位定期同步到MS Dynamics。 使用 _外部人員ID_ 作為filterType，並將MS Dynamics Lead GUID作為filterValue傳遞。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   然後，您可以使用這些欄位的值與MS Dynamics Lead/Contact對象同步。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo領隊</strong></td> 
      <td><strong>MS Dynamics線索/聯繫人欄位</strong></td> 
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

   * Lead REST API的文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}。
   正確使用外部欄位是成功進行非本機同步的關鍵。 如果在某些視圖中未能看到資料，則可能某個欄位未正確同步。 例如，如果潛在客戶在其帳戶下查看MSI構件時未顯示潛在客戶的活動和有趣時刻，則潛在客戶的公司或帳戶可能未正確同步。 在指定外部欄位時執行此潛在顧客的GET請求將幫助您驗證潛在顧客是否正確同步。 此外，Marketo外部銷售人員的電子郵件必須與MS Dynamics中該用戶的電子郵件相匹配。 如果電子郵件不匹配，則資料可能不會顯示在MS Dynamics的「Marketo」頁籤中。
