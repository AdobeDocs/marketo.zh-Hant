---
description: 非原生MS Dynamics整合的Sales Insight - Marketo檔案 — 產品檔案
title: 非原生MS Dynamics整合的Sales Insight
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '1413'
ht-degree: 0%

---

# 非原生MS Dynamics整合的Sales Insight {#sales-insight-for-non-native-ms-dynamics-integrations}

如果您的Adobe Marketo Engage帳戶是透過自訂或非原生整合連線至MS Dynamics，請使用本文來設定Sales Insight。

>[!PREREQUISITES]
>
>* 在開始設定MSI之前，為您的Marketo實例啟用了「MSI非本地」功能。 如果尚未購買，而您已購買功能，請聯絡 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. 如果您尚未購買此功能，請連絡Adobe帳戶團隊（您的客戶經理）。
>* 下載 [用於自定義同步的MSI包](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* MSI安裝程式的MS Dynamics訂閱(我們僅支援 [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} 此時)。
>* Marketo REST API [已成功設定](https://developers.marketo.com/rest-api/){target="_blank"}. 公開的CRUD API將是執行非原生同步的基礎。
>* 閱讀 [此部落格貼文](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} 以便了解對象和關係。


## MSI的非本機同步成功需要以下條件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 將MS Dynamics Sales用戶同步到Marketo。

   MS Dynamics Sales User是擁有MS Dynamics中Lead/Contact的外部用戶。 需要為MS Dynamics Sales用戶更新Marketo銷售人員。 externalSalesPersonId欄位被授權用於Sales Person的更新。

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
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics用戶不區分全局唯一標識符</td> 
      <td><p>將Marketo銷售人員記錄標識為外部MS Dynamics用戶對象。</p><p>要求先同步銷售人員，然後再同步其他對象，以建立正確的關係。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售人員的API檔案： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * 用於同步銷售人員的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target="_blank"}

1. 將MS Dynamics帳戶同步至Marketo。

   需要更新Marketo公司的MS Dynamics帳戶。 此 _externalCompanyId_ 和 _externalSalesPersonId_ 欄位是公司更新的授權欄位。

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
      <td>externalCompanyId</td> 
      <td>MS Dynamics帳戶不區分大小寫全局唯一標識符</td> 
      <td>將Marketo公司記錄標識為外部MS Dynamics帳戶對象。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales用戶不區分全局唯一標識符</td> 
      <td>將Marketo公司記錄標識給外部MS Dynamics Sales User對象（帳戶所有者）。<br><br>也用於Marketo內，將本公司與擁有本公司記錄的銷售人員建立關聯。 設定此欄位之前，必須先同步銷售人員。</td> 
     </tr> 
    </tbody> 
   </table>

   * 適用於公司的API檔案： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * 同步公司的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. 將MS Dynamics銷售線索/聯繫人同步到Marketo。

   您需要為MS Dynamics Lead/Contact上插入Marketo Lead。 此 _externalPersonId_, _externalSalesPersonId_，和 _externalCompanyId_ 欄位是用於Lead的更新的。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo主導欄位</strong></td> 
      <td><strong>MS Dynamics Lead/Contact欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>MS Dynamics Lead/Contact不區分大小寫的全局唯一標識符</td> 
      <td>標識外部MS Dynamics Lead/Contact對象的Marketo Lead記錄。<br><br>這是為MSI非本地導入的新欄位。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales用戶不區分全局唯一標識符</td> 
      <td>標識擁有此銷售機會/聯繫人的外部MS Dynamics Sales User對象。<br><br>也將銷售機會與Marketo的銷售人員相關。 要求先正確同步銷售人員。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識銷售線索/聯繫人所屬的外部MS Dynamics帳戶對象。<br><br>此外，銷售機會記錄也與Marketo的一家公司相關。 強制要求先正確同步MS Dynamics帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

   * 銷售機會的API檔案： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target="_blank"}
   * 同步銷售機會的API檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target="_blank"}

1. 將MS Dynamics Opportunities同步到Marketo。

   您需要為MS Dynamics Opportunity插入Marketo Opportunity。 此 _externalOpportunityId_, _externalCompanyId_，和 _externalSalesPersonId_ 欄位是Opportunity的更新任務。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo機會對象欄位</strong></td> 
      <td><strong>MS Dynamics機會對象欄位</strong></td> 
      <td><strong>說明</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>MS Dynamics Lead/Contact不區分大小寫的全局唯一標識符</td> 
      <td>將Marketo Opportunity記錄標識為外部MS Dynamics Opportunity對象。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帳戶不區分大小寫全局唯一標識符</td> 
      <td>標識此Opportunity所屬的外部MS Dynamics帳戶對象。 <br><br>強制要求先正確同步MS Dynamics帳戶。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales用戶不區分全局唯一標識符</td> 
      <td>標識擁有此Opportunity的外部MS Dynamics Sales User對象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 用於同步商機的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 將MS Dynamics聯繫人角色同步到Marketo。

   然後，可以通過Marketo Opportunity角色同步MS Dynamics Opportunity的MS Dynamics聯繫人角色。 Opportunity Role記錄要求 _externalOpportunityId_, _角色_，和 _leadId_ 欄位。

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
      <td>externalOpportunityId</td> 
      <td>MS Dynamics Opportunity不區分大小寫的全局唯一標識符</td> 
      <td>將Marketo Opportunity角色標識為外部MS Dynamics Opportunity對象。<br><br>強制要求先正確同步MS Dynamics Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>不適用，這會是Marketo潛在客戶ID</td> 
      <td>這會是同步MS Dynamics連絡人的Marketo潛在客戶ID。<br><br>在Marketo中同步連絡人後，您就可以使用MS Dynamics Contact全域不區分大小寫的唯一識別碼作為externalPersonId，並使用Marketo REST API查詢Marketo Lead。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>MS Dynamics聯繫人的角色欄位</td> 
      <td>介紹聯繫人在此機會中的作用。</td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文檔： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 用於同步商機的API文檔： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 將上一個有趣的時刻/MSI計分欄位同步到MS Dynamics。

   將MS Dynamics對象正確同步到Marketo後，您就可以利用MSI功能。 REST API中將公開MSI最後一個有趣的時刻/分數欄位以用於Lead。 這些欄位由MSI計算，並且是只讀的。

   Marketo Lead的「最後有趣的時刻/分數」欄位需要使用REST API Lead端點，定期同步至MS Dynamics。 使用以下項目查詢此端點以找出Marketo銷售機會： _externalPersonId_ 作為filterType，並將MS Dynamics Lead GUID作為filterValue傳入。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   然後，您可以使用這些欄位的值來同步到MS Dynamics Lead/Contact對象。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo主導欄位</strong></td> 
      <td><strong>MS Dynamics Lead/Contact欄位</strong></td> 
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

   * Lead REST API的檔案： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.
   正確使用外部欄位是成功進行非原生同步的關鍵。 如果您在某些檢視中看不到資料，可能會有特定欄位未正確同步。 例如，如果銷售機會的活動和有趣的時刻在其帳戶下查看MSI小工具時未顯示，則銷售機會的公司或帳戶可能未正確同步。 在指定外部欄位時執行此銷售機會的GET請求將有助於您驗證銷售機會是否正確同步。 此外，Marketo中外部銷售人員的電子郵件必須符合MS Dynamics中該使用者的電子郵件。 如果電子郵件不相符，資料可能不會顯示在MS Dynamics的「Marketo」標籤中。
