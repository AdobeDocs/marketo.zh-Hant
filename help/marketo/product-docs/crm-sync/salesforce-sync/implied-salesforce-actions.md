---
unique-page-id: 4719304
description: 隱含的Salesforce動作——行銷檔案——產品檔案
title: 隱含的Salesforce動作
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# 隱含的Salesforce動作 {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

當執行Salesforce特定的流程步驟時，有時會自動執行額外的步驟。 以下是規則，您知道：

當人員目前 *不在 [](http://Salesforce.com)* Salesforce.com中擔任聯絡人或潛在客戶時，這些規則即適用。

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
   <td>將人員同步到<br>SFDC向SFDC宣傳</td> 
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

您可以使用 **** SFDC類型過濾器過濾智慧清單中的SFDC記錄，並將操作符設定為「非空」。 所有SFDC記錄在此欄位中都有值。

請記住，這些自動動作只有在銷售機會目前不在 [Salesforce.com時才會發生](http://Salesforce.com)

Salesforce同步很酷，對吧？
