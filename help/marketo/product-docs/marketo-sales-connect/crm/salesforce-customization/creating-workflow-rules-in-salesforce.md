---
unique-page-id: 14745823
description: 在Salesforce中建立工作流程規則 — Marketo檔案 — 產品檔案
title: 在Salesforce中建立工作流程規則
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 在Salesforce中建立工作流程規則 {#creating-workflow-rules-in-salesforce}

同時使用Marketo Sales Insight(MSI)和Marketo Sales Connect(MSC)時，Salesforce中的MSI Best Bets功能將不會更新。 所有其他MSI功能都照常運作（查看iFrame中有趣的時刻、發送電子郵件、添加到促銷活動等）。 本文提供讓「最佳下注」重新運作的因應措施。

>[!NOTE]
>
>這只會影響使用 **both** MSI和MSE，以及希望在MSI中使用「最佳選擇」功能的用戶。 如果您不需要/使用「最佳下注」，則可以忽略。

## 快速入門 {#getting-started}

解決方法包括建立新的工作流規則，以便將新MSE欄位的值複製到舊的MSI欄位。 您將需要為Contact對象建立四個工作流規則，並在自己的Salesforce實例中為Lead對象建立相同的四個工作流規則。 這可能需要您擁有CRM管理員權限（視您在CRM中的角色和設定而定）。

以下是建議的工作流程規則名稱和每個規則的說明。 這些規則適用於Contact和Lead對象：

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>更新「感興趣的力矩設計」欄位</td> 
   <td><p>複製來源：上次Marketo參與次數<br>複製到：最後一個有趣的時刻Desc</p></td> 
  </tr> 
  <tr> 
   <td>更新「感興趣的力矩類型」欄位</td> 
   <td><p>複製來源：上次Marketo參與類型<br>複製到：最後一個有趣的時刻類型</p></td> 
  </tr> 
  <tr> 
   <td>更新「感興趣的力矩源」欄位</td> 
   <td><p>複製來源：上次Marketo參與來源<br>複製到：最後一個有趣的時刻源</p></td> 
  </tr> 
  <tr> 
   <td>更新「感興趣的時間日期」欄位</td> 
   <td><p>複製來源：上次Marketo參與日期<br>複製到：最後一個有趣的時刻</p></td> 
  </tr> 
 </tbody> 
</table>

## 說明 {#instructions}

1. 按一下 **設定**，搜尋 **工作流程** 選取 **工作流程規則**.

   ![](assets/one-1.png)

1. 選擇 **新規則**.

   ![](assets/two-1.png)

1. 按一下「物件」下拉式清單，然後選取 **銷售機會**，然後按一下 **下一個**.

   ![](assets/three-1.png)

1. 輸入「更新有趣的時刻設計欄位」作為規則名稱。 選擇單選按鈕 **建立，每次編輯**. 在「規則條件」下拉式清單中選取 **公式計算為true**. 搜索並選擇ISCHANGED函式。 接著，反白顯示預設欄位值，然後按一下 **插入欄位**.

   ![](assets/four-1.png)

1. 在「插入欄位」快顯視窗中，選擇 **上次Marketo參與次數** 按一下 **插入**.

   ![](assets/five-1.png)

1. 按一下 **保存和下一步**.

   ![](assets/6.png)

1. 在「新增工作流程動作」下拉式清單中，選取 **新欄位更新**.

   ![](assets/seven.png)

1. 在「名稱」欄位中，輸入「更新有趣的時刻設計欄位」（「唯一名稱」將自動生成）。 在「要更新的欄位」下拉式清單中，選擇 **最後一個有趣的時刻Desc**. 選取 **使用公式來設定新值** 選項按鈕，然後按一下 **顯示公式編輯器**.

   ![](assets/eight.png)

1. 按一下 **插入欄位** 按鈕。

   ![](assets/9a.png)

1. 選擇 **上次Marketo參與次數**，然後按一下 **插入**. 在下一頁，按一下 **儲存**.

   ![](assets/nine.png)

1. 按一下 **完成**.

   ![](assets/twelve.png)

1. 按一下 **啟動** 以開啟工作流程規則。

   ![](assets/thirteen.png)

   在最後一個步驟之後，您可以選取為快速入門區段中列出的其他欄位複製工作流程規則：Desc，類型，源，日期。 在Contact對象中完成四個工作流規則後，對Lead對象重複相同的規則。
