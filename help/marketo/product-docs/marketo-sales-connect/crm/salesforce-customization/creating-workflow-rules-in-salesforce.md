---
unique-page-id: 14745823
description: 在Salesforce中建立工作流程規則 — Marketo檔案 — 產品檔案
title: 在 Salesforce 中建立工作流程規則
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 4%

---

# 在 Salesforce 中建立工作流程規則 {#creating-workflow-rules-in-salesforce}

並行使用Marketo Sales Insight (MSI)和Marketo Sales Connect (MSC)時，[!DNL Salesforce]中的MSI首選功能將不會更新。 所有其他MSI功能都照常運作（在iFrame中檢視有趣的時刻、傳送電子郵件、新增促銷活動等）。 本文提供讓最佳賭注再次運作的因應措施。

>[!NOTE]
>
>這只會影響同時使用&#x200B;**1} MSI和MSE以及想要在MSI中使用Best Bets功能的客戶。**&#x200B;如果您不需要/使用「首選」，可以忽略。

## 快速入門 {#getting-started}

因應措施包括建立新的工作流程規則，將新MSE欄位的值複製到舊MSI欄位。 您需要為連絡人物件建立四個工作流程規則，並為您自己的[!DNL Salesforce]執行個體中的Lead物件建立相同的四個工作流程規則。 您可能需要擁有CRM管理員許可權（視您在CRM中的角色和設定而定）。

以下是工作流程規則的建議名稱及各自的相關說明。 這些套用至[!UICONTROL Contact]和[!UICONTROL Lead]物件：

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

1. 按一下&#x200B;**[!UICONTROL Setup]**&#x200B;之後，搜尋&#x200B;**工作流程**&#x200B;並選取&#x200B;**[!UICONTROL Workflow Rules]**。

   ![](assets/one-1.png)

1. 選取「**[!UICONTROL New Rule]**」。

   ![](assets/two-1.png)

1. 按一下[!UICONTROL Object]下拉式清單並選取&#x200B;**[!UICONTROL Lead]**，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/three-1.png)

1. 輸入「更新有趣的時刻描述欄位」作為[!UICONTROL Rule Name]。 選取選項按鈕&#x200B;**[!UICONTROL created, and every time it’s edited]**。 在[!UICONTROL Rule Criteria]下拉式清單中選取&#x200B;**[!UICONTROL formula evaluates to true]**。 搜尋並選取ISCHANGED函式。 然後，反白顯示預設欄位值並按一下&#x200B;**[!UICONTROL Insert Field]**。

   ![](assets/four-1.png)

1. 在[!UICONTROL Insert Field]快顯視窗中選擇&#x200B;**[!UICONTROL Last Marketo Engagement Desc]**&#x200B;並按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/five-1.png)

1. 按一下「**[!UICONTROL Save & Next]**」。

   ![](assets/6.png)

1. 在[!UICONTROL Add Workflow Action]下拉式清單中，選取&#x200B;**[!UICONTROL New Field Update]**。

   ![](assets/seven.png)

1. 在[!UICONTROL Name]欄位中，輸入「更新有趣的時刻描述欄位」（[!UICONTROL Unique Name]將自動產生）。 從[!UICONTROL Field to Update]下拉式清單中選擇&#x200B;**[!UICONTROL Last Interesting Moment Desc]**。 選取&#x200B;**[!UICONTROL Use a formula to set new value]**&#x200B;選項按鈕，然後按一下&#x200B;**[!UICONTROL Show Formula Editor]**。

   ![](assets/eight.png)

1. 按一下&#x200B;**[!UICONTROL Insert Field]**&#x200B;按鈕。

   ![](assets/9a.png)

1. 選取&#x200B;**[!UICONTROL Last Marketo Engagement Desc]**，然後按一下&#x200B;**[!UICONTROL Insert]**。 在下一頁，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/nine.png)

1. 按一下「**[!UICONTROL Done]**」。

   ![](assets/twelve.png)

1. 按一下&#x200B;**[!UICONTROL Activate]**&#x200B;以開啟工作流程規則。

   ![](assets/thirteen.png)

   在最後一個步驟之後，您可以選擇複製[!UICONTROL Getting Started]區段中所列其他欄位的工作流程規則： Desc、Type、Source、Date。 在您完成[!UICONTROL Contact]物件中的四個工作流程規則後，請對[!UICONTROL Lead]物件重複相同的規則。
