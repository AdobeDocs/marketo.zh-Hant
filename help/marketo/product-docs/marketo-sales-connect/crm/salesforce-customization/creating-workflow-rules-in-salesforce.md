---
unique-page-id: 14745823
description: 在Salesforce - Marketo Docs —— 產品檔案中建立工作流程規則
title: 在Salesforce中建立工作流程規則
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# 在Salesforce中建立工作流程規則 {#creating-workflow-rules-in-salesforce}

當同時使用Marketo Sales Insight(MSI)和Marketo Sales Connect(MSC)時，Salesforce中的MSI最佳押注功能將不會更新。 所有其他MSI功能都正常運作（在iFrame中檢視有趣的時刻、傳送電子郵件、新增至促銷活動等）。 本文提供讓「最佳下注」重新運作的因應措施。

>[!NOTE]
>
>這只會影響同時使用 **MSI** 和MSE，以及想要在MSI中使用「最佳押注」功能的客戶。 如果您不需要／使用「最佳賭注」，可以忽略。

## 快速入門 {#getting-started}

因應措施包括建立新的工作流程規則，將新MSE欄位的值複製到舊的MSI欄位。 您將需要為Contact對象建立四個工作流規則，並在自己的Salesforce實例中為Lead對象建立相同的四個工作流規則。 這可能需要您擁有CRM管理員權限（視您在CRM中的角色和設定而定）。

以下是建議的工作流程規則名稱和每個規則的說明。 這些項目適用於Contact和Lead對象：

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>更新有趣的力矩設計欄位</td> 
   <td><p>複製來源：上一個行銷人員參與<br>DescCopy，您可以：最後一個有趣的時刻Desc</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的力矩類型欄位</td> 
   <td><p>複製來源：上一個行銷人員參與<br>類型複製至：最後一個有趣的力矩類型</p></td> 
  </tr> 
  <tr> 
   <td>更新「有趣的時刻來源」欄位</td> 
   <td><p>複製來源：Last Marketo Engagement<br>SourceCopy到：最後一個有趣的時刻來源</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的時刻日期欄位</td> 
   <td><p>複製來源：Last Marketo Engagement<br>DateCopy至：最後一個有趣的時刻</p></td> 
  </tr> 
 </tbody> 
</table>

## 說明 {#instructions}

1. 按一下「 **設定**」後，搜尋「工 **作流程** 」並選 **取「工作流規則**」。

   ![](assets/one-1.png)

1. 選擇 **新規則**。

   ![](assets/two-1.png)

1. 按一下「物件」下拉式清單，然後選 **取「銷售線索**」，然後按一 **下「下一步**」。

   ![](assets/three-1.png)

1. 輸入「更新有趣的時刻描述欄位」作為規則名稱。 選取已建立的 **選項按鈕，並在每次編輯時加以選取**。 在「規則條件」下拉式清單中，選取 **公式評估為true**。 搜索並選擇ISCHANGED函式。 然後，反白顯示預設欄位值，然後按一 **下「插入欄位**」。

   ![](assets/four-1.png)

1. 在「插入欄位」彈出式選單中，選擇「上次行銷 **人員參與設計」** ，然後按一 **下「插入」**。

   ![](assets/five-1.png)

1. 按一 **下「儲存並下一步**」。

   ![](assets/6.png)

1. 在「新增工作流程動作」下拉式清單中，選取「新 **增欄位更新」**。

   ![](assets/seven.png)

1. 在「名稱」欄位中，輸入「更新有趣的時刻描述欄位」（「唯一名稱」會自動產生）。 在「要更新的欄位」下拉式清單中，選擇「最 **後一個有趣的時刻設計**」。 選擇「使 **用公式設定新值」單選按鈕** ，然後按一下「 **顯示公式編輯器」**。

   ![](assets/eight.png)

1. 按一下「 **插入欄位** 」按鈕。

   ![](assets/9a.png)

1. 選取「 **上次行銷人員參與設計」**，然後按一下「 **插入」**。 在下一頁，按一下「 **儲存**」。

   ![](assets/nine.png)

1. 按一 **下完成**。

   ![](assets/twelve.png)

1. 按一 **下「啟動** 」以開啟工作流程規則。

   ![](assets/thirteen.png)

   在最後一個步驟後，您可以選擇複製「快速入門」區段中所列其他欄位的工作流程規則：設計、類型、來源、日期。 完成Contact對象中的四個工作流規則後，請對Lead對象重複相同的規則。

