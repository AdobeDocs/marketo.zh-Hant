---
description: 將銷售活動屬性記錄到Salesforce - Marketo檔案 — 產品檔案
title: 將銷售活動屬性記錄至 Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 14%

---

# 將銷售活動屬性記錄到[!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

Salesforce管理員可以手動將自訂活動欄位新增到[!DNL Salesforce]。

1. 在您的[!DNL Salesforce]帳戶中，按一下&#x200B;**[!UICONTROL Setup]**。

1. 在快速搜尋欄位中搜尋「活動自訂欄位」，然後按一下它。

1. 按一下「**[!UICONTROL New]**」。

1. 根據下表，選取與您要新增的欄位對應的資料型別，然後按一下&#x200B;**[!UICONTROL Next]**。

1. 輸入欄位名稱和標籤，對應到您要新增的欄位。

下表各欄的說明：

* **欄位標籤**： UI中顯示的欄位名稱（此名稱可以自訂，以提高團隊的可讀性）
* **欄位名稱**：欄位的技術名稱（請確定您輸入的欄位名稱符合下表中的欄位名稱）
* **API名稱**： API欄位的技術名稱（請確定您輸入的API名稱符合下表中的API名稱）
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
  <td>[!UICONTROL Call Outcomes]</td>
  <td>mktosales_call_output</td>
  <td>mktosales_call_output__c</td>
  <td>文字</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Call Reasons]</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>文字</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Local Presence ID]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Recording URL]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign Current Step]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign URL]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Attachment Viewed]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Clicked]</td>
  <td>mse_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Replied]</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Status]</td>
  <td>mse_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>文字</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template URL]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email URL]</td>
  <td>mse_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Viewed]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>核取方塊</td>
  <td></td>
 </tr>
</table>
