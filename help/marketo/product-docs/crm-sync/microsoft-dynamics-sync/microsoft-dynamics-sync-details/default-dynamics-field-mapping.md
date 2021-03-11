---
description: 預設動態欄位對應——行銷人員至檔案——產品檔案
title: 預設動態欄位映射
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# 預設動態欄位映射{#default-dynamics-field-mapping}

當您最初將Marketo帳戶與Microsoft同步時，Marketo會自動在您的內建Dynamics和Marketo欄位之間建立這些關聯。  Marketo也會同步您的Lead、Accounts、Opportunity和Contacts上的自訂欄位。

## 銷售線索欄位{#lead-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo Field</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API名稱</th> 
  </tr> 
  <tr> 
   <td>Microsoft建立日期</td> 
   <td>建立於</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>問候語</td> 
   <td>問候語</td> 
   <td>問候語</td> 
  </tr> 
  <tr> 
   <td>First</td> 
   <td>名字</td> 
   <td>名字</td> 
  </tr> 
  <tr> 
   <td>中間</td> 
   <td>中間名</td> 
   <td>米德倫娜</td> 
  </tr> 
  <tr> 
   <td>上次</td> 
   <td>姓氏</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>電子郵件</td> 
   <td>電子郵件</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>職稱</td> 
   <td>職稱</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>電話</td> 
   <td>商務電話</td> 
   <td>電話1</td> 
  </tr> 
  <tr> 
   <td>行動裝置</td> 
   <td>行動電話</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>傳真</td> 
   <td>傳真</td> 
   <td>傳真</td> 
  </tr> 
  <tr> 
   <td>地址</td> 
   <td>街1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>城市</td> 
   <td>城市</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>州</td> 
   <td>州／省</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>國家／地區</td> 
   <td>國家／地區</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>郵遞區號</td> 
   <td>郵遞區號</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>人員來源</td> 
   <td>銷售線索來源</td> 
   <td>引導原始碼</td> 
  </tr> 
  <tr> 
   <td>人員狀態</td> 
   <td>狀態</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>狀態原因</td> 
   <td>狀態原因</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>人員附註</td> 
   <td>說明</td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td>不要呼叫</td> 
   <td>不允許電話呼叫</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>取消訂閱</td> 
   <td>不大量傳送電子郵件</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>人員評分</td> 
   <td>評分</td> 
   <td>優質程式碼</td> 
  </tr> 
  <tr> 
   <td>Microsoft地址2</td> 
   <td>街2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft地址3</td> 
   <td>街3號</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Email</td> 
   <td>不允許電子郵件</td> 
   <td>donomail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Fax</td> 
   <td>不允許傳真</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Microsoft不傳送行銷資料</td> 
   <td>行銷資料</td> 
   <td>多諾森姆</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>家庭電話</td> 
   <td>電話2</td> 
  </tr> 
  <tr> 
   <td>Microsoft首選的聯繫方法</td> 
   <td>首選的聯繫方法</td> 
   <td>preferredcontactmethodcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft主題</td> 
   <td>主題</td> 
   <td>主旨</td> 
  </tr> 
 </tbody> 
</table>

## 連絡人欄位{#contact-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo Field</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API名稱</th> 
  </tr> 
  <tr> 
   <td>Microsoft建立日期</td> 
   <td>建立於</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>問候語</td> 
   <td>問候語</td> 
   <td>問候語</td> 
  </tr> 
  <tr> 
   <td>First</td> 
   <td>名字</td> 
   <td>名字</td> 
  </tr> 
  <tr> 
   <td>中間</td> 
   <td>中間名</td> 
   <td>米德倫娜</td> 
  </tr> 
  <tr> 
   <td>上次</td> 
   <td>姓氏</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>電子郵件</td> 
   <td>電子郵件</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>職稱</td> 
   <td>職稱</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>電話</td> 
   <td>商務電話</td> 
   <td>電話1</td> 
  </tr> 
  <tr> 
   <td>行動裝置</td> 
   <td>行動電話</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>地址</td> 
   <td>地址1:街1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>城市</td> 
   <td>地址1:城市</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>州</td> 
   <td>地址1:州／省</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>國家／地區</td> 
   <td>地址1:國家／地區</td> 
   <td>address1_country</td> 
   <tr> 
   <td>郵遞區號</td> 
   <td>地址1:郵遞區號</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>人員狀態</td> 
   <td>狀態</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>狀態原因</td> 
   <td>狀態原因</td> 
   <td>statuscode</td> 
  </tr> 
   <tr> 
   <td>不要呼叫</td> 
   <td>不允許電話呼叫</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>取消訂閱</td> 
   <td>不大量傳送電子郵件</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft地址2</td> 
   <td>地址1:街2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Microsoft地址3</td> 
   <td>地址1:街3號</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Email</td> 
   <td>不允許電子郵件</td> 
   <td>donomail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>家庭電話</td> 
   <td>電話2</td> 
  </tr> 
  <tr> 
   <td>Microsoft首選的聯繫方法</td> 
   <td>首選的聯繫方法</td> 
   <td>preferredcontactmethodcode</td> 
  </tr> 
 </tbody> 
</table>

## 帳戶欄位{#account-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo Field</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API名稱</th> 
  </tr> 
  <tr> 
   <td>帳戶(a)</td> 
   <td>帳戶</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>帳單地址</td> 
   <td>地址1:街1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>帳單城市</td> 
   <td>地址1:城市</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>帳單國家／地區</td> 
   <td>地址1:國家／地區</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>帳單郵遞區號</td> 
   <td>地址1:郵遞區號</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft帳單地址2</td> 
   <td>地址1:街2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft帳單地址3</td> 
   <td>地址1:街3號</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>主手機</td> 
   <td>主手機</td> 
   <td>電話1</td> 
  </tr> 
  <tr> 
   <td>業務類型</td> 
   <td>業務類型</td> 
   <td>businestypecode</td> 
  </tr> 
  <tr> 
   <td>Microsoft帳號</td> 
   <td>帳號</td> 
   <td>accountnumber</td> 
  </tr> 
  <tr> 
   <td>Microsoft公司狀態</td> 
   <td>狀態</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>年收入</td> 
   <td>年收入</td> 
   <td>收入</td> 
  </tr> 
  <tr> 
   <td>公司說明</td> 
   <td>說明</td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td>產業</td> 
   <td>產業</td> 
   <td>業界程式碼</td> 
  </tr> 
  <tr> 
   <td>SIC代碼</td> 
   <td>SIC代碼</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>網站</td> 
   <td>網站</td> 
   <td>網站</td> 
  </tr> 
 </tbody> 
</table>

## Marketo中的Microsoft相關系統欄位（只讀）{#microsoft-related-system-fields-in-marketo}

這些欄位是在Marketo中建立，但客戶無法調整。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo Field</th> 
   <th>說明</th> 
  </tr> 
  <tr> 
   <td>Microsoft類型</td> 
   <td>潛在客戶或聯絡人。 如果空白，則銷售線索僅作為Marketto中的人員存在</td> 
  </tr> 
  <tr> 
   <td>Microsoft建立日期</td> 
   <td>在MS Dynamics中建立的日期（可以與在Marketto中建立的日期不同）</td> 
  </tr> 
  <tr> 
   <td>已刪除Microsoft</td> 
   <td>以前在微軟工作的人，但被刪除，現在只住在Marketo</td> 
  </tr> 
 </tbody> 
</table>
