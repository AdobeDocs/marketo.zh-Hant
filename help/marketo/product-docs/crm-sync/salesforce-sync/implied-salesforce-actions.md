---
unique-page-id: 4719304
description: 隱含的Salesforce動作 — Marketo檔案 — 產品檔案
title: 隱含的Salesforce動作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# 隱含的Salesforce動作 {#implied-salesforce-actions}

當Salesforce特定的流程步驟執行時，有時會自動執行額外的步驟。 規則如下，您知道：

這些規則將適用 _當人員目前不在時 [Salesforce.com](https://Salesforce.com)_ 作為聯絡人或潛在客戶。

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
   <td>變更SFDC促銷活動中的狀態</td> 
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

您可以使用以下工具來篩選掉智慧清單中的SFDC記錄： **SFDC型別** 運運算元設為「非空白」的篩選。 所有SFDC記錄在此欄位中都有一個值。

請記住，這些自動動作只有在潛在客戶目前不在時才會發生 [Salesforce.com](https://salesforce.com)
