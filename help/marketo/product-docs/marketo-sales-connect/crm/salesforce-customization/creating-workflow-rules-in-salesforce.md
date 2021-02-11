---
unique-page-id: 14745823
description: 在Salesforce - Marketo Docs —— 產品檔案中建立工作流程規則
title: 在Salesforce中建立工作流程規則
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# 在Salesforce {#creating-workflow-rules-in-salesforce}中建立工作流程規則

當同時使用Marketo Sales Insight(MSI)和Marketo Sales Connect(MSC)時，Salesforce中的MSI最佳押注功能將不會更新。 所有其他MSI功能都正常運作（在iFrame中檢視有趣的時刻、傳送電子郵件、新增至促銷活動等）。 本文提供讓「最佳下注」重新運作的因應措施。

>[!NOTE]
>
>這只會影響同時使用&#x200B;**** MSI和MSE，以及想要在MSI中使用「最佳押注」功能的客戶。 如果您不需要／使用「最佳賭注」，可以忽略。

## 開始使用{#getting-started}

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
   <td><p>複製來源：上次行銷人員參與設計<br>複製至：最後一個有趣的時刻Desc</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的力矩類型欄位</td> 
   <td><p>複製來源：上次行銷人員參與類型<br>複製至：最後一個有趣的力矩類型</p></td> 
  </tr> 
  <tr> 
   <td>更新「有趣的時刻來源」欄位</td> 
   <td><p>複製來源：上次行銷人員參與來源<br>複製至：最後一個有趣的時刻來源</p></td> 
  </tr> 
  <tr> 
   <td>更新有趣的時刻日期欄位</td> 
   <td><p>複製來源：上次行銷人員參與日期<br>複製至：最後一個有趣的時刻</p></td> 
  </tr> 
 </tbody> 
</table>

## 說明{#instructions}

1. 按一下&#x200B;**Setup**&#x200B;後，搜索&#x200B;**Workflow**&#x200B;並選擇&#x200B;**Workflow Rules**。

   ![](assets/one-1.png)

1. 選擇&#x200B;**新規則**。

   ![](assets/two-1.png)

1. 按一下「Object（對象）」下拉式清單並選擇&#x200B;**Lead** ，然後按一下&#x200B;**Next**。

   ![](assets/three-1.png)

1. 輸入「更新有趣的時刻描述欄位」作為規則名稱。 選取已建立的選項按鈕&#x200B;**，並在每次編輯**&#x200B;時加以選取。 在「規則條件」下拉式清單中，選擇&#x200B;**公式評估為true**。 搜索並選擇ISCHANGED函式。 然後，選中預設欄位值，然後按一下「插入欄位」。****

   ![](assets/four-1.png)

1. 在「插入欄位」彈出式選單中，選擇&#x200B;**上次行銷人員參與設計**，然後按一下「插入&#x200B;****」。

   ![](assets/five-1.png)

1. 按一下&#x200B;**保存和下一步**。

   ![](assets/6.png)

1. 在「添加工作流操作」下拉式清單中，選擇「新建欄位更新」。****

   ![](assets/seven.png)

1. 在「名稱」欄位中，輸入「更新有趣的時刻描述欄位」（「唯一名稱」會自動產生）。 在「要更新的欄位」下拉式清單中，選擇&#x200B;**最後一個有趣時刻說明**。 選擇&#x200B;**使用公式設定新值**&#x200B;單選按鈕，然後按一下&#x200B;**顯示公式編輯器**。

   ![](assets/eight.png)

1. 按一下&#x200B;**插入欄位**&#x200B;按鈕。

   ![](assets/9a.png)

1. 選擇&#x200B;**上次行銷參與設計**，然後按一下&#x200B;**插入**。 在下一頁，按一下&#x200B;**保存**。

   ![](assets/nine.png)

1. 按一下&#x200B;**Done**。

   ![](assets/twelve.png)

1. 按一下「啟動」以開啟工作流程規則。****

   ![](assets/thirteen.png)

   在最後一個步驟後，您可以選擇複製「快速入門」區段中所列其他欄位的工作流程規則：設計、類型、來源、日期。 完成Contact對象中的四個工作流規則後，請對Lead對象重複相同的規則。
