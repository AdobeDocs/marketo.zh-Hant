---
unique-page-id: 45417125
description: '[!DNL Sales Insight]非原生整合 [!DNL Salesforce] Marketo檔案 — 產品檔案'
title: '[!DNL Sales Insight]非原生整合 [!DNL Salesforce] 整合'
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---

# 非原生[!DNL Sales Insight]整合的[!DNL Salesforce] {#sales-insight-for-non-native-salesforce-integrations}

如果您的Adobe Marketo Engage帳戶是透過自訂或非原生整合連線至[!DNL Salesforce]，請使用本文來設定[!DNL Sales Insight]。

>[!PREREQUISITES]
>
>* 開始設定MSI之前，已為您的Marketo執行個體啟用「MSI非原生」功能。 如果不是，而且您已購買此功能，請連絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。 如果您尚未購買此功能，請聯絡Adobe客戶團隊（您的客戶經理）。
>* 已設定[MSI封裝的Salesforce帳戶](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}。
>* Marketo REST API [已成功設定](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。 公開的CRUD API將是執行非原生同步的基礎。
>* 請閱讀[此部落格](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"}，以瞭解物件與關聯性。
>* 設定[!DNL Salesforce]物件以顯示18個字元不區分大小寫的全域唯一識別碼，而非15個字元區分大小寫的全域唯一識別碼。

>[!NOTE]
>
>Marketo MSI管理面板中的REST API設定無法用於非原生同步。

## MSI成功的非原生同步需要下列專案 {#successful-non-native-sync-for-msi-requires-the-following}

1. 將[!DNL Salesforce]銷售使用者同步至Marketo。

   [!DNL Salesforce]銷售使用者是擁有[!DNL Salesforce]中潛在客戶/聯絡人的外部使用者。 需要為[!DNL Salesforce]銷售使用者更新Marketo銷售人員。 *externalSalesPersonId*&#x200B;欄位必須用於更新銷售人員。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo銷售人員欄位</strong></td>
        <td><strong><span class="dnl">Salesforce</span>銷售使用者欄位</strong></td>
      <td><strong>說明</strong></td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span>銷售使用者不區分大小寫的全域唯一識別碼</td>
      <td><p>識別外部<span class="dnl">Salesforce</span>銷售使用者物件的Marketo銷售人員記錄。</p><p>在同步其他物件之前，必須先同步銷售人員，才能建立適當的關係。</p></td>
     </tr>
    </tbody>
   </table>

   * 銷售人員的API檔案： [https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * 同步處理銷售人員的API檔案： [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. 將[!DNL Salesforce]帳戶同步至Marketo。

   [!DNL Salesforce]帳戶需要更新Marketo公司。 _externalCompanyId_&#x200B;和&#x200B;_externalSalesPersonId_&#x200B;欄位是公司更新插入的必要欄位。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo公司欄位</strong></td>
        <td><strong><span class="dnl">Salesforce</span>帳戶欄位</strong></td>
      <td><strong>說明</strong></td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td><span class="dnl">Salesforce</span>帳戶不區分大小寫的全域唯一識別碼</td>
        <td>識別外部<span class="dnl">Salesforce</span>帳戶物件的Marketo公司記錄。</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span>銷售使用者不區分大小寫的全域唯一識別碼</td>
        <td>向身為帳戶擁有者的外部<span class="dnl">Salesforce</span>銷售使用者物件識別Marketo公司記錄。<br><br>也在Marketo內用來將公司與擁有公司紀錄的銷售人員建立關聯。 在設定此欄位之前，必須先同步銷售人員。</td>
     </tr>
    </tbody>
   </table>

   * 公司的API檔案： [https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * 同步處理公司的API檔案： [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. 將[!DNL Salesforce]銷售機會/聯絡人同步至Marketo。

   您必須為[!DNL Salesforce]銷售機會/聯絡人更新插入Marketo銷售機會。 _externalPersonId_、_externalSalesPersonId_&#x200B;和&#x200B;_externalCompanyId_&#x200B;欄位已強製為潛在客戶更新插入。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo潛在客戶欄位</strong></td>
        <td><strong><span class="dnl">Salesforce</span>銷售機會/聯絡人欄位</strong></td>
      <td><strong>說明</strong></td>
     </tr>
     <tr>
      <td>externalPersonId</td>
        <td><span class="dnl">Salesforce</span>銷售機會/聯絡人不區分大小寫的全域唯一識別碼</td>
        <td>識別外部<span class="dnl">Salesforce</span>銷售機會/連絡人物件的Marketo銷售機會記錄。<br><br>這是為MSI Non-Native引進的新欄位。</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span>銷售使用者不區分大小寫的全域唯一識別碼</td>
        <td>識別擁有此銷售機會/連絡人的外部<span class="dnl">Salesforce</span>銷售使用者物件。<br><br>也會將潛在客戶與Marketo中的銷售人員建立關聯。 必須先正確同步銷售人員。</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td><span class="dnl">Salesforce</span>帳戶不區分大小寫的全域唯一識別碼</td>
        <td>識別潛在客戶/連絡人所屬的外部<span class="dnl">Salesforce</span>帳戶物件。<br><br>也將潛在客戶記錄關聯至Marketo中的公司。 必須先正確同步Salesforce帳戶。</td>
     </tr>
    </tbody>
   </table>

   * 潛在客戶的API檔案： [https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/leads)
   * 同步潛在客戶的API檔案： [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. 將[!DNL Salesforce]個機會同步至Marketo。

   您必須為[!DNL Salesforce]個機會更新插入Marketo機會。 _externalOpportunityId_、_externalCompanyId_&#x200B;和&#x200B;_externalSalesPersonId_&#x200B;欄位必須執行商機的更新插入。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo機會物件欄位</strong></td>
        <td><strong><span class="dnl">Salesforce</span>機會物件欄位</strong></td>
      <td><strong>說明</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
      <td>Salesforce銷售機會/聯絡人不區分大小寫的全域唯一識別碼</td>
      <td>識別外部Marketo機會物件的Salesforce機會記錄。</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td><span class="dnl">Salesforce</span>帳戶不區分大小寫的全域唯一識別碼</td>
        <td>識別此機會所屬的外部<span class="dnl">Salesforce</span>帳戶物件。 <br><br>強制要求<span class="dnl">Salesforce</span>帳戶必須先正確同步。</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span>銷售使用者不區分大小寫的全域唯一識別碼</td>
        <td>識別擁有此商機的外部<span class="dnl">Salesforce</span>銷售使用者物件。 </td>
     </tr>
    </tbody>
   </table>

   * 機會的API檔案： [https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * 同步商機的API檔案： [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. 將[!DNL Salesforce]連絡人角色同步至Marketo。

   接著，可以透過Marketo機會角色同步[!DNL Salesforce]機會的[!DNL Salesforce]聯絡人角色。 機會角色記錄授權&#x200B;_externalOpportunityId_、_role_&#x200B;和&#x200B;_leadId_&#x200B;欄位。

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
        <td><span class="dnl">Salesforce</span>機會不區分大小寫的全域唯一識別碼</td>
        <td>識別外部<span class="dnl">Salesforce</span>機會物件的Marketo機會角色。<br><br>規定<span class="dnl">Salesforce</span>機會必須先正確同步。</td>
     </tr>
     <tr>
      <td>leadId</td>
      <td>不適用，這將會是Marketo銷售機會ID</td>
        <td>這會是同步的<span class="dnl">Salesforce</span>連絡人的Marketo銷售機會ID。<br><br>聯絡人在Marketo中同步後，您就可以使用<span class="dnl">Salesforce</span>不區分大小寫的聯絡人全域唯一識別碼做為externalPersonId，並使用Marketo REST API查詢Marketo銷售機會。</td>
     </tr>
     <tr>
      <td>角色</td>
        <td><span class="dnl">Salesforce</span>連絡人的角色欄位</td>
      <td>說明此機會的連絡人角色。</td>
     </tr>
    </tbody>
   </table>

   * 機會的API檔案： [https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * 同步商機的API檔案： [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. 將上一個有趣的時刻/MSI評分欄位同步到SFDC。

   將您的[!DNL Salesforce]物件正確同步至Marketo後，您就可以使用MSI功能。 MSI最後一個有趣的時刻/評分欄位將會在潛在客戶的REST API中公開。 這些欄位由MSI計算，且為唯讀。

   Marketo銷售機會的「上次有趣的時刻/評分」欄位需要使用REST API銷售機會端點定期同步至[!DNL Salesforce]。 使用&#x200B;_externalPersonId_&#x200B;作為filterType，並將[!DNL Salesforce]銷售機會GUID傳入filterValue，查詢此Marketo銷售機會的端點。

   | GET /rest/v1/leads.json？filterType=externalPersonId&amp;filterValues=salesforceLeadId1，salesforceLeadId2 |
   |---|

   然後，您可以使用這些欄位的值，同步至您的[!DNL Salesforce]銷售機會/連絡人物件。

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Marketo潛在客戶欄位</strong></td>
        <td><strong><span class="dnl">Salesforce</span>銷售機會/聯絡人欄位</strong></td>
      <td><strong>說明</strong></td>
     </tr>
     <tr>
      <td>msiLastInterestedMomentType</td>
      <td>標籤：上一個有趣的時刻型別<br>名稱： Last_Interested_Moment_Type__c</td>
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
      <td>潛在客戶最後有趣時刻的說明</td>
     </tr>
     <tr>
      <td>msiLastInterestedMomentSource</td>
      <td><p>標籤：Source上一個有趣的時刻</p><p>名稱：Last_Interested_Moment_Source__c</p></td>
      <td>潛在客戶最後有趣時刻的Source</td>
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

   Lead REST API的檔案： [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}。

   正確使用外部欄位是成功非原生同步化的關鍵。 如果您在某些檢視中看不到資料，可能是因為某個欄位未正確同步。 例如，如果在檢視「帳戶」底下的MSI Widget時，沒有顯示潛在客戶的活動和有趣的時刻，則可能是潛在客戶的公司或帳戶未正確同步。 在指定外部欄位時對此潛在客戶執行GET要求，將協助您驗證該潛在客戶是否已正確同步。 此外，Marketo中外部銷售人員的電子郵件必須與Salesforce中該使用者的電子郵件相符。 如果電子郵件不符，資料可能不會顯示在Salesforce的Marketo標籤中。
