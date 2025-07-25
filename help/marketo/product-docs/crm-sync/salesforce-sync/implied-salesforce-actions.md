---
unique-page-id: 4719304
description: 隱含的Salesforce動作 — Marketo檔案 — 產品檔案
title: 隱含的Salesforce動作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# 隱含的Salesforce動作 {#implied-salesforce-actions}

當[!DNL Salesforce]特定的流程步驟執行時，有時會自動執行額外的步驟。 規則如下，您知道：

當人員目前不是在[Salesforce.com](https://Salesforce.com){target="_blank"}中作為連絡人或潛在客戶時，將套用這些規則。

<table> 
 <thead> 
  <tr> 
   <th>Marketo流程步驟</th> 
   <th>自動動作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新增至SFDC Campaign</td> 
   <td>將人員同步至SFDC</td> 
  </tr> 
  <tr> 
   <td>在SFDC Campaign中變更狀態</td> 
   <td>將人員同步至SFDC<br>新增至SFDC Campaign</td> 
  </tr> 
  <tr> 
   <td>變更擁有者</td> 
   <td><p>將人員同步至SFDC</p></td> 
  </tr> 
  <tr> 
   <td>轉換人員</td> 
   <td><p>將人員同步至SFDC</p></td> 
  </tr> 
  <tr> 
   <td>建立任務</td> 
   <td>將人員同步至SFDC</td> 
  </tr> 
 </tbody> 
</table>

您可以使用運運算元設為&quot;**[!UICONTROL SFDC Type]**&quot;的[!UICONTROL is not empty]篩選條件，篩選掉智慧清單中的SFDC記錄。 所有SFDC記錄在此欄位中都有一個值。

請記住，只有當潛在客戶目前不在[Salesforce.com](https://salesforce.com){target="_blank"}中時，才會發生這些自動動作
