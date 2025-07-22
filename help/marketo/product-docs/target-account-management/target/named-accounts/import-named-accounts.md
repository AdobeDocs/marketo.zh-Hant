---
unique-page-id: 12615800
description: 匯入[!UICONTROL Named Accounts] - Marketo檔案 — 產品檔案
title: 匯入[!UICONTROL Named Accounts]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 匯入[!UICONTROL Named Accounts] {#import-named-accounts}

CSV中已經滿載了潛在的目標帳戶嗎？ 將它們直接匯入TAM！

1. 按一下&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Import Named Accounts]**。

   ![](assets/inaone.png)

1. 將會開啟新視窗。 按一下&#x200B;**[!UICONTROL Browse]**，然後選取您要匯入的具名帳戶檔案。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >在您的檔案中，提供[儘可能多的資訊](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes)。 您只能新增實體資訊；Marketo不會計算任何內容（例如Pipeline）。 若要根據CRM帳戶建立具名帳戶，只需將帳戶名稱和CRM ID從您的CRM匯出至CSV檔案、使用「帳戶名稱」選項，並在匯入過程中對應CRM ID即可。 若要正確將CRM帳戶連結至具名帳戶，您必須提供CRM帳戶的正確名稱。

1. 從兩種重複資料刪除模式中選擇：帳戶名稱或網域名稱。 在此範例中，我們將選擇「帳戶」。 按一下&#x200B;**[!UICONTROL Modes]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL By Account Name]**。

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >如果您選擇&#x200B;**[!UICONTROL By Domain Name]**，則必須同時包含具名帳戶和網域欄位。

1. 若要選擇您的具名帳戶要新增至哪個帳戶清單，請按一下&#x200B;**[!UICONTROL Account List]**&#x200B;下拉式清單，然後進行選取。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >您也可以在下拉式方塊中輸入名稱，即可建立全新的[!UICONTROL Account List]。

1. 若要傳送匯入通知，請按一下&#x200B;**[!UICONTROL Send Alert To]**&#x200B;下拉式清單，然後選取Marketo使用者。 您&#x200B;_無法_&#x200B;手動輸入電子郵件地址。

   ![](assets/inafive-2.png)

1. 按一下「**[!UICONTROL Next]**」。

   ![](assets/inasix-2.png)

1. 連按兩下&#x200B;**[!UICONTROL Marketo Field]**&#x200B;下拉式清單並選取適當的欄位，以對應每個欄位。 完成時，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/inaseven.png)

   成功！

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >「檢查匯入狀態」只會顯示活動的最後三天。

刪除重複資料[!UICONTROL by Account Name]的情況：

<table> 
 <tbody> 
  <tr> 
   <td><strong>正在匯入具有現有<span class="uicontrol">具名帳戶</span>名稱的記錄</strong></td> 
   <td><p>我們將更新現有的記錄</p></td> 
  </tr> 
  <tr> 
   <td><strong>正在匯入具有新<span class="uicontrol">具名帳戶</span>名稱的記錄</strong></td> 
   <td>我們將建立新記錄</td> 
  </tr> 
 </tbody> 
</table>

刪除重複資料[!UICONTROL by Domain Name]的情況：

<table> 
 <tbody> 
  <tr> 
   <td><strong>使用新帳戶名稱與新網域名稱匯入記錄</strong></td> 
   <td>我們將使用提供的資訊建立新的<span class="uicontrol">具名帳戶</span></td> 
  </tr> 
  <tr> 
   <td><strong>使用現有帳戶名稱和現有網域名稱匯入記錄</strong></td> 
   <td>我們將更新現有的<span class="uicontrol">具名帳戶</span></td> 
  </tr> 
   <tr> 
   <td><strong>使用新帳戶名稱和現有網域名稱匯入記錄</strong></td> 
   <td>我們將新帳戶名稱附加至符合網域名稱的現有<span class="uicontrol">具名帳戶</span>，並更新其他資訊（例如產業、州等）</td> 
  </tr> 
  <tr> 
   <td><strong>正在匯入具有現有<span class="uicontrol">具名帳戶</span>名稱與新網域名稱的記錄</strong></td> 
   <td>我們將新網域名稱附加至符合帳戶名稱的現有<span class="uicontrol">具名帳戶</span>，並更新其他資訊（例如產業、狀態等）</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當Marketo附加具名帳戶時，我們會更新規則（在幕後），以允許我們識別應該成為[!UICONTROL Named Account]一部分的人。 範例：如果您將「IBM」更新為「IBM， USA」，具有任一公司名稱的人員將會與[!UICONTROL Named Account]相關聯。

如果Marketo找到我們視為重複專案的記錄，我們只會處理第一個記錄。
