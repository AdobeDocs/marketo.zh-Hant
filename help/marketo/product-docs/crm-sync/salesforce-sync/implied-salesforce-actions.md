---
unique-page-id: 4719304
description: 瞭解哪些Salesforce流程步驟會觸發自動將人員同步到SFDC或其他動作。 瞭解新增至行銷活動、變更擁有者、建立任務和轉換人員的規則。
title: 隱含的 Salesforce 動作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/lI3sRqk1if-UZ7DARSrGXXM485ZjZnlqDGb4si2wvi0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 158
ht-degree: 23%

---

# 隱含的 Salesforce 動作 {#implied-salesforce-actions}

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
   <td>新增至 SFDC 行銷活動</td>
   <td>將人員同步至 SFDC</td>
  </tr>
  <tr>
   <td>在 SFDC 行銷活動中變更狀態</td>
   <td>將人員同步至SFDC<br>新增至SFDC Campaign</td>
  </tr>
  <tr>
   <td>變更所有者</td>
   <td><p>將人員同步至 SFDC</p></td>
  </tr>
  <tr>
   <td>轉換人員</td>
   <td><p>將人員同步至 SFDC</p></td>
  </tr>
  <tr>
   <td>建立工作</td>
   <td>將人員同步至 SFDC</td>
  </tr>
 </tbody>
</table>

您可以使用運運算元設為&quot;[!UICONTROL is not empty]&quot;的&#x200B;**[!UICONTROL SFDC Type]**&#x200B;篩選條件，篩選掉智慧清單中的SFDC記錄。 所有SFDC記錄在此欄位中都有一個值。

請記住，只有當潛在客戶目前不在[Salesforce.com](https://salesforce.com){target="_blank"}中時，才會發生這些自動動作
