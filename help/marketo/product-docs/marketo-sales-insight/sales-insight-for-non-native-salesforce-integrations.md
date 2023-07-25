---
unique-page-id: 45417125
description: 非原生Salesforce整合的Sales Insight - Marketo檔案 — 產品檔案
title: 非原生Salesforce整合的Sales Insight
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# 非原生Salesforce整合的Sales Insight {#sales-insight-for-non-native-salesforce-integrations}

如果您的Adobe Marketo Engage帳戶是透過自訂或非原生整合連線至Salesforce，請使用本文章設定Sales Insight。

>[!PREREQUISITES]
>
>* 在您開始設定MSI之前，已為您的Marketo執行個體啟用「MSI非原生」功能。 如果不是，而且您已購買此功能，請聯絡 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. 如果您尚未購買此功能，請聯絡Adobe客戶團隊（您的客戶經理）。
>* 具有的Salesforce帳戶 [MSI封裝設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* MARKETO REST API [已成功設定](https://developers.marketo.com/rest-api/){target="_blank"}. 公開的CRUD API將是執行非原生同步的基礎。
>* 讀取 [此部落格](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} 以瞭解物件和關係。
>* 設定Salesforce物件以顯示18個字元不區分大小寫的全域唯一識別碼，而非15個字元區分大小寫的全域唯一識別碼。

>[!NOTE]
>
>Marketo MSI管理面板中的REST API設定無法用於非原生同步。

## MSI的非原生同步必須具備下列條件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 將Salesforce銷售使用者同步至Marketo。

   Salesforce銷售使用者是擁有Salesforce中潛在客戶/聯絡人的外部使用者。 需要為Salesforce銷售使用者更新Marketo銷售人員。 此 *externalSalesPersonId* 欄位必須用於更新銷售人員。

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
      <td>Salesforce銷售使用者不區分大小寫的全域唯一識別碼</td> 
      <td><p>識別外部Salesforce銷售使用者物件的Marketo銷售人員記錄。</p><p>在同步其他物件之前，必須先同步銷售人員，才能建立適當的關係。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 適用於銷售人員的API檔案： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * 同步銷售人員的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Sales_Persones/syncSalesPersonesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persones/syncSalesPersonesUsingPOST){target="_blank"}

1. 將Salesforce帳戶同步至Marketo。

   Salesforce帳戶需要更新Marketo公司。 此 _externalCompanyId_ 和 _externalSalesPersonId_ 欄位必須用於公司的更新。

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
      <td>識別外部Salesforce帳戶物件的Marketo公司記錄。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce銷售使用者不區分大小寫的全域唯一識別碼</td> 
      <td>向身為帳戶擁有者的外部Salesforce銷售使用者物件識別Marketo公司記錄。<br><br>也用於在Marketo中將公司與擁有公司紀錄的銷售人員建立關聯。 在設定此欄位之前，必須先同步銷售人員。</td> 
     </tr> 
    </tbody> 
   </table>

   * 適用於公司的API檔案： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * 同步公司的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. 將Salesforce銷售機會/聯絡人同步至Marketo。

   您需要為Salesforce銷售機會/聯絡人更新插入Marketo銷售機會。 此 _externalPersonId_， _externalSalesPersonId_、和 _externalCompanyId_ 欄位必須用於Lead的更新。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo潛在客戶欄位</strong></td> 
      <td><strong>Salesforce銷售機會/聯絡人欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Salesforce銷售機會/聯絡人不區分大小寫的全域唯一識別碼</td> 
      <td>識別外部Salesforce銷售機會/聯絡人物件的Marketo銷售機會記錄。<br><br>這是為「MSI非原生」引入的新欄位。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce銷售使用者不區分大小寫的全域唯一識別碼</td> 
      <td>識別擁有此銷售機會/連絡人的外部Salesforce銷售使用者物件。<br><br>也將Lead與Marketo中的銷售人員相關聯。 必須先正確同步銷售人員。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帳戶不區分大小寫的全域唯一識別碼</td> 
      <td>識別潛在客戶/聯絡人所屬的外部Salesforce帳戶物件。<br><br>還將潛在客戶記錄關聯到Marketo中的公司。 必須先正確同步Salesforce帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

   * 潛在客戶的API檔案： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * 同步潛在客戶的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 將Salesforce Opportunities同步至Marketo。

   您需要為Salesforce機會更新插入Marketo機會。 此 _externalOpportunityId_， _externalCompanyId_、和 _externalSalesPersonId_ 欄位必須用於更新插入商機。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會物件欄位</strong></td> 
      <td><strong>Salesforce機會物件欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce銷售機會/聯絡人不區分大小寫的全域唯一識別碼</td> 
      <td>識別外部Salesforce機會物件的Marketo機會記錄。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帳戶不區分大小寫的全域唯一識別碼</td> 
      <td>識別此機會所屬的外部Salesforce帳戶物件。 <br><br>必須先正確同步Salesforce帳戶。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce銷售使用者不區分大小寫的全域唯一識別碼</td> 
      <td>識別擁有此Opportunity的外部Salesforce銷售使用者物件。 </td> 
     </tr> 
    </tbody> 
   </table>

   * 機會的API檔案： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 同步商機的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 將Salesforce連絡人角色同步至Marketo。

   接著，可以透過Marketo Opportunity Role同步Salesforce機會的Salesforce聯絡人角色。 機會角色記錄會授權 _externalOpportunityId_， _角色_、和 _leadId_ 欄位。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會角色欄位</strong></td> 
      <td><strong>Salesforce聯絡人角色欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce機會不區分大小寫的全域唯一識別碼</td> 
      <td>向外部Salesforce機會物件識別Marketo機會角色。<br><br>必須先正確同步Salesforce Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>不適用，這將會是Marketo銷售機會ID</td> 
      <td>這會是同步的Salesforce連絡人的Marketo銷售機會ID。<br><br>聯絡人在Marketo中同步後，您可以使用Salesforce聯絡人不區分大小寫的全域唯一識別碼作為externalPersonId，並使用Marketo REST API查詢Marketo Lead。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>Salesforce連絡人的「角色」欄位</td> 
      <td>說明此機會的聯絡人角色。</td> 
     </tr> 
    </tbody> 
   </table>

   * 機會的API檔案： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 同步商機的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 將上一個有趣的時刻/MSI評分欄位同步至SFDC。

   將Salesforce物件正確同步至Marketo後，您就可以利用MSI功能。 潛在客戶的REST API會顯示「MSI上次有趣的時刻/評分」欄位。 這些欄位由MSI計算，且為唯讀。

   Marketo銷售機會的「最後有趣時刻/評分」欄位需要使用REST API銷售機會端點定期同步至Salesforce。 使用以下專案查詢Marketo銷售機會的此端點 _externalPersonId_ 作為filterType，並以filterValue傳入Salesforce銷售機會GUID。

   | GET/rest/v1/leads.json？filterType=externalPersonId&amp;filterValues=salesforceLeadId1，salesforceLeadId2 |
   |---|

   然後，您可以使用這些欄位的值來同步至您的Salesforce銷售機會/聯絡人物件。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo潛在客戶欄位</strong></td> 
      <td><strong>Salesforce銷售機會/聯絡人欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentType</td> 
      <td>標籤：上一個有趣的時刻型別<br>名稱：Last_Interested_Moment_Type__c</td> 
      <td>潛在客戶最後有趣時刻的型別</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDate</td> 
      <td><p>標籤：上一個有趣的時刻日期</p><p>名稱：Last_Interested_Moment_Date__c</p></td> 
      <td>潛在客戶最後一個有趣時刻的日期</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDesc</td> 
      <td><p>標籤：上一個有趣時刻說明</p><p>名稱：Last_Interested_Moment_Desc__c</p></td> 
      <td>潛在客戶最後一個有趣時刻的說明</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentSource</td> 
      <td><p>標籤：上一個有趣時刻來源</p><p>名稱：Last_Interested_Moment_Source__c</p></td> 
      <td>潛在客戶最後一個有趣時刻的來源</td> 
     </tr> 
     <tr> 
      <td>優先順序</td> 
      <td><p>標籤：參與</p><p>名稱： Priority__c</p></td> 
      <td>潛在客戶的優先順序</td> 
     </tr> 
     <tr> 
      <td>相對急迫性</td> 
      <td><p>標籤：相對緊急值</p><p>名稱：Urgency_Value__c</p></td> 
      <td>潛在客戶的相對急迫性</td> 
     </tr> 
     <tr> 
      <td>相對評分</td> 
      <td><p>標籤：相對評分值</p><p>名稱：Relative_Score_Value__c</p></td> 
      <td>潛在客戶的相對評分</td> 
     </tr> 
    </tbody> 
   </table>

   Lead REST API的檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   正確使用外部欄位是成功非原生同步的關鍵。 如果您在某些檢視中看不到資料，可能是因為某個欄位未正確同步。 例如，如果潛在客戶在其帳戶下方檢視MSI Widget時，未顯示其活動和有趣的時刻，則可能是潛在客戶的公司或帳戶未正確同步。 在指定外部欄位時執行此銷售機會的GET要求，將協助您驗證該銷售機會是否已正確同步。 此外，Marketo中外部銷售人員的電子郵件必須與Salesforce中該使用者的電子郵件相符。 如果電子郵件不相符，資料可能不會顯示在Salesforce的Marketo索引標籤中。
