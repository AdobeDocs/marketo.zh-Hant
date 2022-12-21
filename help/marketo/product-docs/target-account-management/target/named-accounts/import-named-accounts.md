---
unique-page-id: 12615800
description: 匯入指定帳戶 — Marketo檔案 — 產品檔案
title: 導入命名帳戶
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# 導入命名帳戶 {#import-named-accounts}

已有CSV檔案包含潛在目標帳戶嗎？ 將它們直接導入TAM!

1. 按一下 **新增** 下拉式清單並選取 **導入命名帳戶**.

   ![](assets/inaone.png)

1. 將會開啟新窗口。 按一下 **瀏覽**，然後選擇要導入的已命名帳戶的檔案。

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >在您的檔案中，提供 [資訊量](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) 盡可能。 您只能添加字母資訊；Marketo不會計算任何項目（即管道）。 若要根據CRM帳戶建立指定帳戶，只需將帳戶名稱和CRM ID從您的CRM匯出至CSV檔案、使用「帳戶名稱」選項，並在匯入程式期間對應CRM ID。 若要將CRM帳戶正確連結至指定帳戶，您必須提供CRM帳戶的確切名稱。

1. 從兩種重複資料消除模式中選擇：帳戶名稱或網域名稱。 在此範例中，我們將選擇「帳戶」。 按一下 **模式** 下拉式清單並選取 **按帳戶名稱**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >如果您選擇 **按域模式**，必須同時包含指定帳戶和網域欄位。

1. 若要選擇您指定的帳戶要新增至的帳戶清單，請按一下 **帳戶清單** 下拉式清單中選取。

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >您也可以在下拉式方塊中輸入帳戶清單名稱，以建立全新的帳戶清單。

1. 若要傳送匯入通知，請按一下 **將警報發送到** 下拉式清單中選取Marketo使用者。 您 _不能_ 手動輸入電子郵件地址。

   ![](assets/inafive-2.png)

1. 按一下 **下一個**.

   ![](assets/inasix-2.png)

1. 按兩下 **Marketo欄位** 下拉式清單並選取適當欄位。 按一下 **下一個** 時才能使用。

   ![](assets/inaseven.png)

   成功!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >「檢查匯入狀態」只會顯示活動的最近三天。

按帳戶名稱刪除重複資料的情況：

<table> 
 <tbody> 
  <tr> 
   <td><strong>正在導入具有現有命名帳戶名的記錄</strong></td> 
   <td><p>我們將更新現有記錄</p></td> 
  </tr> 
  <tr> 
   <td><strong>正在導入具有新命名帳戶名的記錄</strong></td> 
   <td>我們將創造新記錄</td> 
  </tr> 
 </tbody> 
</table>

按域名刪除重複資料的情況：

<table> 
 <tbody> 
  <tr> 
   <td><strong>正在使用新帳戶名和新域名導入記錄</strong></td> 
   <td>我們將使用提供的資訊建立新的指定帳戶</td> 
  </tr> 
  <tr> 
   <td><strong>正在導入具有現有帳戶名和現有域名的記錄</strong></td> 
   <td>我們將更新現有的指定帳戶</td> 
  </tr> 
   <tr> 
   <td><strong>正在使用新帳戶名和現有域名導入記錄</strong></td> 
   <td>我們會將新帳戶名稱附加至符合網域名稱的現有指定帳戶，並更新其他資訊（例如產業、州等）</td> 
  </tr> 
  <tr> 
   <td><strong>正在導入具有現有命名帳戶名和新域名的記錄</strong></td> 
   <td>我們會將新網域名稱附加至符合帳戶名稱的現有指定帳戶，並更新其他資訊（例如產業、州等）</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當Marketo附加指名帳戶時，我們會更新規則（幕後），以便我們識別應屬於指名帳戶的人員。 範例：如果您將&quot;IBM&quot;更新為&quot;IBM, USA&quot;，則具有任一公司名稱的人員將與指定帳戶相關聯。

如果Marketo找到我們視為重複的記錄，我們只會處理第一個記錄。
