---
unique-page-id: 45417125
description: 非原生Salesforce整合的Sales Insight - Marketo檔案 — 產品檔案
title: 非原生Salesforce整合的銷售分析
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: fb663ddf4c0021f258317636fbc7794e8172ab7e
workflow-type: tm+mt
source-wordcount: '1400'
ht-degree: 0%

---

# 非原生Salesforce整合的銷售分析 {#sales-insight-for-non-native-salesforce-integrations}

如果您的Adobe Marketo Engage帳戶是透過自訂或非原生整合連線至Salesforce，請使用本文來設定Sales Insight。

>[!PREREQUISITES]
>
>* 在開始設定MSI之前，為您的Marketo實例啟用了「MSI非本地」功能(如果沒有，並且您已購買了該功能，請聯繫 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} — 如果您尚未購買此功能，請連絡您的客戶成功經理)。
>* 具有 [MSI包設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}。
>* Marketo REST API [已成功設定](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}。 公開的CRUD API將是執行非原生同步的基礎。
>* 閱讀 [此部落格貼文](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;}，以了解物件和關係。
>* 設定Salesforce對象以顯示18個不區分大小寫的全局唯一標識符，而不是15個區分大小寫的全局唯一標識符。


>[!NOTE]
>
>Marketo MSI管理面板中的REST API配置不能用於非本機同步。

## MSI的非本機同步成功需要以下條件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 將Salesforce Sales使用者同步至Marketo。

   Salesforce Sales User是在Salesforce中擁有Lead/Contacts的外部用戶。 需要為Salesforce Sales用戶更新Marketo銷售人員。 此 *externalSalesPersonId* 欄位被授權用於更新銷售人員。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo銷售人員欄位</strong></td> 
      <td><strong>Salesforce銷售用戶欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td><p>將「Marketo銷售人員」記錄標識為外部「Salesforce銷售用戶」對象。</p><p>要求先同步銷售人員，然後再同步其他對象，以建立正確的關係。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售人員的API檔案： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;}
   * 用於同步銷售人員的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target=&quot;_blank&quot;}

1. 將Salesforce帳戶同步至Marketo。

   需要更新Marketo公司的Salesforce帳戶。 此 _externalCompanyId_ 和 _externalSalesPersonId_ 欄位是公司更新的授權欄位。

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
      <td>Salesforce帳戶不區分大小寫的全局唯一標識符</td> 
      <td>將Marketo公司記錄識別為外部Salesforce帳戶物件。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>將Marketo公司記錄標識給外部Salesforce Sales User對象（帳戶所有者）。<br><br>也用於Marketo內，將本公司與擁有本公司記錄的銷售人員建立關聯。 設定此欄位之前，必須先同步銷售人員。</td> 
     </tr> 
    </tbody> 
   </table>

   * 適用於公司的API檔案： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;}
   * 同步公司的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target=&quot;_blank&quot;}

1. 將Salesforce銷售機會/聯繫人同步到Marketo。

   您需要為Salesforce銷售機會/聯繫人更新Marketo銷售機會。 此 _externalPersonId_, _externalSalesPersonId_，和 _externalCompanyId_ 欄位是用於Lead的更新的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo主導欄位</strong></td> 
      <td><strong>Salesforce銷售機會/聯繫欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Salesforce銷售機會/聯繫人不區分大小寫的全局唯一標識符</td> 
      <td>將Marketo銷售機會記錄標識為外部Salesforce銷售機會/聯繫人對象。<br><br>這是為MSI非本地導入的新欄位。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識擁有此銷售機會/聯繫人的外部Salesforce Sales User對象。<br><br>也將銷售機會與Marketo的銷售人員相關。 要求先正確同步銷售人員。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帳戶不區分大小寫的全局唯一標識符</td> 
      <td>標識銷售線索/聯繫人所屬的外部Salesforce帳戶對象。<br><br>此外，銷售機會記錄也與Marketo的一家公司相關。 強制要求先正確同步Salesforce帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售機會的API檔案： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * 同步銷售機會的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 將Salesforce Opportunity同步至Marketo。

   您需要為Salesforce Opportunity添加Marketo Opportunity。 此 _externalOpportunityId_, _externalCompanyId_，和 _externalSalesPersonId_ 欄位是Opportunity的更新任務。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會對象欄位</strong></td> 
      <td><strong>Salesforce機會對象欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce銷售機會/聯繫人不區分大小寫的全局唯一標識符</td> 
      <td>將Marketo Opportunity記錄標識到外部Salesforce Opportunity對象。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帳戶不區分大小寫的全局唯一標識符</td> 
      <td>標識此Opportunity所屬的外部Salesforce帳戶對象。 <br><br>強制要求先正確同步Salesforce帳戶。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales用戶不區分大小寫全局唯一標識符</td> 
      <td>標識擁有此Opportunity的外部Salesforce Sales User對象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * 用於同步商機的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target=&quot;_blank&quot;}

1. 將Salesforce連絡人角色同步至Marketo。

   然後，可以通過Marketo Opportunity角色同步Salesforce Opportunity的Salesforce聯繫人角色。 Opportunity Role記錄要求 _externalOpportunityId_, _角色_，和 _leadId_ 欄位。

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
      <td>externalOpportunityId</td> 
      <td>Salesforce Opportunity不區分大小寫的全局唯一標識符</td> 
      <td>將Marketo Opportunity角色標識到外部Salesforce Opportunity對象。<br><br>要求先正確同步Salesforce Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>不適用，這會是Marketo潛在客戶ID</td> 
      <td>這會是同步Salesforce連絡人的Marketo潛在客戶ID。<br><br>在Marketo中同步連絡人後，您就可以使用Salesforce Contact不區分大小寫的全域唯一識別碼作為externalPersonId，並使用Marketo REST API查詢Marketo Lead。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>Salesforce聯繫人的角色欄位</td> 
      <td>介紹聯繫人在此機會中的作用。</td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * 用於同步商機的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target=&quot;_blank&quot;}

1. 將上一個有趣的時刻/MSI計分欄位同步到SFDC。

   將Salesforce對象正確同步到Marketo後，您就可以利用MSI功能。 REST API中將公開MSI最後一個有趣的時刻/分數欄位以用於Lead。 這些欄位由MSI計算，並且是只讀的。

   Marketo Lead的「最後有趣的時刻/分數」欄位需要使用REST API Lead端點定期同步至Salesforce。 使用以下項目查詢此端點以找出Marketo銷售機會： _externalPersonId_ 作為filterType，並將Salesforce Lead GUID作為filterValue傳入。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   然後，您可以使用這些欄位的值來同步至您的Salesforce銷售機會/聯繫人對象。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo主導欄位</strong></td> 
      <td><strong>Salesforce銷售機會/聯繫欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentType</td> 
      <td>標籤：最後一個有趣的時刻類型<br>名稱：Last_Interest_Moment_Type__c</td> 
      <td>Lead的最後有趣時刻的類型</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentDate</td> 
      <td><p>標籤：最後一個有趣的時刻</p><p>名稱：Last_Interest_Moment_Date__c</p></td> 
      <td>銷售機會最後有趣時刻的日期</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentDesc</td> 
      <td><p>標籤：最後一個有趣的時刻描述</p><p>名稱：Last_Interest_Moment_Desc__c</p></td> 
      <td>Lead最後一個有趣時刻的說明</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestMomentSource</td> 
      <td><p>標籤：最後一個有趣的時刻源</p><p>名稱：Last_Interest_Moment_Source__c</p></td> 
      <td>Lead最後有趣時刻的來源</td> 
     </tr> 
     <tr> 
      <td>優先順序</td> 
      <td><p>標籤：參與</p><p>名稱：優先順序__c</p></td> 
      <td>銷售機會的優先順序</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>標籤：相對緊急值</p><p>名稱：Urgency_Value__c</p></td> 
      <td>Lead的相對緊急性</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>標籤：相對計分值</p><p>名稱：Relative_Score_Value__c</p></td> 
      <td>銷售線索的相對評分</td> 
     </tr> 
    </tbody> 
   </table>

   Lead REST API的檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}。

   正確使用外部欄位是成功進行非原生同步的關鍵。 如果您在某些檢視中看不到資料，可能會有特定欄位未正確同步。 例如，如果銷售機會的活動和有趣的時刻在其帳戶下查看MSI小工具時未顯示，則銷售機會的公司或帳戶可能未正確同步。 在指定外部欄位時執行此銷售機會的GET請求將有助於您驗證銷售機會是否正確同步。 此外，Marketo中外部銷售人員的電子郵件必須符合Salesforce中該使用者的電子郵件。 如果電子郵件不相符，資料可能不會顯示在Salesforce的「Marketo」標籤中。
