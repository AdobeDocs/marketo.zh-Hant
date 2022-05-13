---
description: 將銷售活動屬性記錄到Salesforce -Marketo文檔 — 產品文檔
title: 將銷售活動屬性記錄到Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 222b0692998be1fd15dc6465af1da627e1c32683
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 2%

---

# 將銷售活動屬性記錄到Salesforce {#logging-sales-activity-attributes-to-salesforce}

Salesforce管理員可以手動將自定義活動欄位添加到Salesforce。

1. 在Salesforce帳戶中，按一下 **設定**。

1. 在快速搜索欄位中搜索「活動自定義欄位」，然後按一下。

1. 按一下 **新建**。

1. 根據下表選擇與要添加的欄位對應的資料類型，然後按一下 **下一個**。

1. 輸入與要添加的欄位對應的欄位名稱和標籤。

下表中各列的說明：

* **欄位標籤**:UI中顯示的欄位名稱（可以自定義此名稱，以提高團隊的可讀性）
* **欄位名稱**:欄位的技術名稱（確保輸入的欄位名稱與下表中的欄位名稱匹配）
* **API名稱**:API欄位的技術名稱（確保輸入的API名稱與下表中的API名稱匹配）
* **資料類型**:欄位類型
* **大小**:文本欄位的大小

<table>
 <tr>
  <th>欄位標籤</th>
  <th>欄位名稱</th>
  <th>API名稱</th>
  <th>資料類型</th>
  <th>大小</th>
 </tr>
 <tr>
  <td>Marketo銷售呼叫本地存在ID</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID_c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo銷售呼叫錄制URL</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售活動</td>
  <td>MSE_市場活動</td>
  <td>MSE_Campign_c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo銷售活動當前步驟</td>
  <td>MSE_Current_Campign_Step</td>
  <td>MSE_Current_Campaign_Step_c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo銷售活動URL</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaig_Details_Link_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件附件已查看</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>複選框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件已按一下</td>
  <td>已按一下MSE_</td>
  <td>MSE_Clicked__c</td>
  <td>複選框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件已回復</td>
  <td>MSE_Rexpled</td>
  <td>MSE_Rexpled__c</td>
  <td>複選框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件狀態</td>
  <td>MSE_E-mail_Status</td>
  <td>MSE_E-mail_Status__c</td>
  <td>文字</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件模板</td>
  <td>MSE_模板</td>
  <td>MSE_Template_c</td>
  <td>文字</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件模板URL</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件URL</td>
  <td>MSE_詳細資訊</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo銷售電子郵件已查看</td>
  <td>已查看MSE_</td>
  <td>MSE_已查看__c</td>
  <td>複選框</td>
  <td></td>
 </tr>
</table>
