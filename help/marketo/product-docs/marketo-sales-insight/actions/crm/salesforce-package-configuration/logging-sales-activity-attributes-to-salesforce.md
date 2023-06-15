---
description: 將銷售活動屬性記錄到Salesforce - Marketo檔案 — 產品檔案
title: 將銷售活動屬性記錄到Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 5%

---

# 將銷售活動屬性記錄到Salesforce {#logging-sales-activity-attributes-to-salesforce}

Salesforce管理員可以手動將自訂活動欄位新增到Salesforce。

1. 在您的Salesforce帳戶中，按一下 **設定**.

1. 在快速搜尋欄位中搜尋「活動自訂欄位」，然後按一下它。

1. 按一下 **新增**.

1. 根據下表，選取與您要新增的欄位對應的資料型別，然後按一下 **下一個**.

1. 輸入與您要新增的欄位對應的欄位名稱和標籤。

下表各欄的說明：

* **欄位標籤**：欄位名稱顯示在UI中（此名稱可自訂以提高團隊的可讀性）
* **欄位名稱**：欄位的技術名稱（請確定您輸入的欄位名稱符合下表中的欄位名稱）
* **API名稱**：欄位的技術名稱（請確定您輸入的API名稱符合下表中的API名稱）
* **資料型別**：欄位型別
* **大小**：文字欄位的大小

<table>
 <tr>
  <th>欄位標籤</th>
  <th>欄位名稱</th>
  <th>API名稱</th>
  <th>資料類型</th>
  <th>大小</th>
 </tr>
  <tr>
  <td>呼叫結果</td>
  <td>mktosales_call_outcome</td>
  <td>mktosales_call_outcome__c</td>
  <td>文字</td>
  <td>50</td>
 </tr>
 <tr>
  <td>來電原因</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>文字</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Marketo銷售電話當地狀態ID</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo銷售電話記錄URL</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo促銷活動</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo促銷活動目前步驟</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo促銷活動URL</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>已檢視的Marketo銷售電子郵件附件</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件已點按</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件已回覆</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件狀態</td>
  <td>mse_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>文字</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件範本</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件範本URL</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件URL</td>
  <td>mse_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>已檢視的Marketo銷售電子郵件</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
</table>
