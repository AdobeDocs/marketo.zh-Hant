---
unique-page-id: 4719304
description: 隱含的Salesforce動作 — Marketo檔案 — 產品檔案
title: 隱含的Salesforce動作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# 隱含的Salesforce動作 {#implied-salesforce-actions}

當Salesforce特定的流程步驟運行時，有時會自動執行額外的步驟。 規則如下：

這些規則將適用 _當該人目前不在 [Salesforce.com](https://Salesforce.com)_ 作為聯繫人或領導。

<table> 
 <thead> 
  <tr> 
   <th>Marketo流量步驟</th> 
   <th>自動動作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>添加到SFDC促銷活動</td> 
   <td>將人員同步到SFDC</td> 
  </tr> 
  <tr> 
   <td>更改SFDC促銷活動中的狀態</td> 
   <td>將人員同步到SFDC<br>添加到SFDC促銷活動</td> 
  </tr> 
  <tr> 
   <td>更改所有者</td> 
   <td><p>將人員同步到SFDC</p></td> 
  </tr> 
  <tr> 
   <td>轉換人員</td> 
   <td><p>將人員同步到SFDC</p></td> 
  </tr> 
  <tr> 
   <td>建立任務</td> 
   <td>將人員同步到SFDC</td> 
  </tr> 
 </tbody> 
</table>

您可以使用 **SFDC類型** 將運算子設為「非空白」的篩選。 此欄位中的所有SFDC記錄都有值。

請記住，這些自動動作只有在銷售機會目前不在 [Salesforce.com](https://salesforce.com)
