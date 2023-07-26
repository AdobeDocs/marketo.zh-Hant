---
unique-page-id: 12615800
description: 匯入具名帳戶 — Marketo檔案 — 產品檔案
title: 匯入具名帳戶
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# 匯入具名帳戶 {#import-named-accounts}

CSV中已經滿載了潛在的目標帳戶嗎？ 將它們直接匯入TAM！

1. 按一下 **新增** 下拉式清單並選取 **匯入具名帳戶**.

   ![](assets/inaone.png)

1. 將會開啟新視窗。 按一下 **瀏覽**，然後選取您要匯入之具名帳戶的檔案。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >在您的檔案中，提供 [儘可能多的資訊](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) 越多越好。 您只能新增實體資訊；Marketo不會計算任何內容（例如Pipeline）。 若要根據CRM帳戶建立具名帳戶，只需將帳戶名稱和CRM ID從您的CRM匯出至CSV檔案、使用「帳戶名稱」選項，並在匯入過程中對應CRM ID即可。 若要正確將CRM帳戶連結至具名帳戶，您必須提供CRM帳戶的正確名稱。

1. 從兩種重複資料刪除模式中選擇：帳戶名稱或網域名稱。 在此範例中，我們將選擇「帳戶」。 按一下 **模式** 下拉式清單並選取 **依帳戶名稱**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >如果您選擇 **依網域模式**，必須包含具名帳戶和網域欄位。

1. 若要選擇您的指定帳戶要新增至哪個帳戶清單，請按一下 **帳戶清單** 下拉式清單，然後進行選取。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >您也可以直接在下拉式方塊中輸入名稱，建立全新的帳戶清單。

1. 若要傳送匯入通知，請按一下 **傳送警報至** 下拉式清單，然後選取Marketo使用者。 您 _無法_ 手動輸入電子郵件地址。

   ![](assets/inafive-2.png)

1. 按一下 **下一個**.

   ![](assets/inasix-2.png)

1. 連按兩下 **Marketo欄位** 下拉式清單，並選取適當的欄位。 按一下 **下一個** 完成時。

   ![](assets/inaseven.png)

   成功!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >「檢查匯入狀態」只會顯示活動的最後三天。

依帳戶名稱進行重複資料刪除的案例：

<table> 
 <tbody> 
  <tr> 
   <td><strong>使用現有的具名帳戶名稱匯入記錄</strong></td> 
   <td><p>我們將更新現有的記錄</p></td> 
  </tr> 
  <tr> 
   <td><strong>使用新的具名帳戶名稱匯入記錄</strong></td> 
   <td>我們將建立新記錄</td> 
  </tr> 
 </tbody> 
</table>

依網域名稱重複資料刪除的案例：

<table> 
 <tbody> 
  <tr> 
   <td><strong>使用新帳戶名稱與新網域名稱匯入記錄</strong></td> 
   <td>我們將使用提供的資訊建立新的具名帳戶</td> 
  </tr> 
  <tr> 
   <td><strong>使用現有帳戶名稱和現有網域名稱匯入記錄</strong></td> 
   <td>我們將更新現有的具名帳戶</td> 
  </tr> 
   <tr> 
   <td><strong>使用新帳戶名稱和現有網域名稱匯入記錄</strong></td> 
   <td>我們將新帳戶名稱附加至符合網域名稱的現有指定帳戶，並更新其他資訊（例如產業、州等）</td> 
  </tr> 
  <tr> 
   <td><strong>使用現有的具名帳戶名稱與新網域名稱匯入記錄</strong></td> 
   <td>我們會將新網域名稱附加至符合帳戶名稱的現有具名帳戶，並更新其他資訊（例如產業、州等）</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當Marketo附加具名帳戶時，我們會更新規則（在幕後），以允許我們識別應屬於具名帳戶的人員。 範例：如果您將「IBM」更新為「IBM， USA」，具有任一公司名稱的人員將與具名帳戶相關聯。

如果Marketo找到我們視為重複專案的記錄，我們只會處理第一個記錄。
