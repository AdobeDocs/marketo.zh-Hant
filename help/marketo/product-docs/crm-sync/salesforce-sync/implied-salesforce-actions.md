---
unique-page-id: 4719304
description: 隱含的Salesforce動作——行銷檔案——產品檔案
title: 隱含的Salesforce動作
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---


# 隱含的Salesforce動作{#implied-salesforce-actions}

當執行Salesforce特定的流程步驟時，有時會自動執行額外的步驟。 以下是規則，您知道：

當人員目前不在[Salesforce.com](https://Salesforce.com)_中時，這些規則將適用_。

<table> 
 <thead> 
  <tr> 
   <th>行銷人員流程步驟</th> 
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
   <td>變更擁有者</td> 
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

您可以使用&#x200B;**SFDC類型**&#x200B;過濾器過濾智慧清單中的SFDC記錄，並將運算子設定為「不空」。 所有SFDC記錄在此欄位中都有值。

請記住，這些自動動作只有在銷售線索目前不在[Salesforce.com](https://salesforce.com)時才會發生
