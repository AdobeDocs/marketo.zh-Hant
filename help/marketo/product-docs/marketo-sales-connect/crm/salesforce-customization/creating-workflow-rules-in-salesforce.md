---
unique-page-id: 14745823
description: 在Salesforce中建立工作流程規則 — Marketo檔案 — 產品檔案
title: 在Salesforce中建立工作流程規則
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 在Salesforce中建立工作流程規則 {#creating-workflow-rules-in-salesforce}

並行使用Marketo Sales Insight (MSI)和Marketo Sales Connect (MSC)時，Salesforce中的MSI首選功能將不會更新。 所有其他MSI功能都照常運作（在iFrame中檢視有趣的時刻、傳送電子郵件、新增促銷活動等）。 本文提供讓最佳賭注再次運作的因應措施。

>[!NOTE]
>
>這只會影響同時使用&#x200B;**1&rbrace; MSI和MSE以及想要在MSI中使用Best Bets功能的客戶。**&#x200B;如果您不需要/使用「首選」，可以忽略。

## 快速入門 {#getting-started}

因應措施包括建立新的工作流程規則，將新MSE欄位的值複製到舊MSI欄位。 您需要為Contact物件建立四個工作流程規則，並為您自己的Salesforce例項中的Lead物件建立相同的四個工作流程規則。 您可能需要擁有CRM管理員許可權（視您在CRM中的角色和設定而定）。

以下是工作流程規則的建議名稱及各自的相關說明。 這些適用於Contact與Lead物件：

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>更新有趣的時刻描述欄位</td> 
   <td><p>複製自：上次Marketo參與度描述<br>複製至：上次有趣的時刻描述</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的時刻型別欄位</td> 
   <td><p>複製自：上次Marketo參與型別<br>複製至：上次有趣的時刻型別</p></td> 
  </tr> 
  <tr> 
   <td>更新「有趣的時刻」Source欄位</td> 
   <td><p>複製自：上次Marketo參與Source<br>複製至：上一個有趣的時刻Source</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的時刻日期欄位</td> 
   <td><p>複製自：上次Marketo參與日期<br>複製至：上次有趣的時刻日期</p></td> 
  </tr> 
 </tbody> 
</table>

## 指示 {#instructions}

1. 按一下&#x200B;**設定**&#x200B;後，搜尋&#x200B;**工作流程**&#x200B;並選取&#x200B;**工作流程規則**。

   ![](assets/one-1.png)

1. 選取&#x200B;**新規則**。

   ![](assets/two-1.png)

1. 按一下「物件」下拉式清單，選取&#x200B;**銷售機會**，然後按一下&#x200B;**下一步**。

   ![](assets/three-1.png)

1. 輸入「更新有趣的時刻描述欄位」作為規則名稱。 選取已建立的選項按鈕&#x200B;**，並且每次都進行編輯**。 在「規則條件」下拉式清單中，選取&#x200B;**公式評估為true**。 搜尋並選取ISCHANGED函式。 接著，反白顯示預設欄位值，然後按一下&#x200B;**插入欄位**。

   ![](assets/four-1.png)

1. 在「插入欄位」快顯視窗中，選擇&#x200B;**上次Marketo參與描述**，然後按一下&#x200B;**插入**。

   ![](assets/five-1.png)

1. 按一下&#x200B;**儲存與下一步**。

   ![](assets/6.png)

1. 在[新增工作流程動作]下拉式清單中，選取&#x200B;**新欄位更新**。

   ![](assets/seven.png)

1. 在「名稱」欄位中，輸入「更新有趣的時刻描述欄位」（唯一名稱會自動產生）。 在[要更新的欄位]下拉式清單中，選擇&#x200B;**上一個有趣的時刻描述**。 選取&#x200B;**使用公式設定新值**&#x200B;選項按鈕，然後按一下&#x200B;**顯示公式編輯器**。

   ![](assets/eight.png)

1. 按一下&#x200B;**插入欄位**&#x200B;按鈕。

   ![](assets/9a.png)

1. 選取&#x200B;**最後一個Marketo參與摘要**，然後按一下&#x200B;**插入**。 在下一頁，按一下&#x200B;**儲存**。

   ![](assets/nine.png)

1. 按一下&#x200B;**完成**。

   ![](assets/twelve.png)

1. 按一下&#x200B;**啟動**&#x200B;以開啟工作流程規則。

   ![](assets/thirteen.png)

   在最後一個步驟之後，您可以選擇複製「快速入門」區段中其他欄位的工作流程規則：說明、型別、Source、日期。 完成Contact物件中的四個工作流程規則後，對Lead物件重複相同的步驟。
