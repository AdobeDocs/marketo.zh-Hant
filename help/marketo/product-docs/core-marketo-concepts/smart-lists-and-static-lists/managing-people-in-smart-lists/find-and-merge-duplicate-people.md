---
unique-page-id: 557339
description: 尋找及合併重複人員 — Marketo檔案 — 產品檔案
title: 找到重複人員並將其合併
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 3456e4d0d9fdcd4590884d9a5b15ef206fcff875
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 3%

---

# 找到重複人員並將其合併 {#find-and-merge-duplicate-people}

當有新人員進入系統時，Marketo Engage會自動刪除重複專案。 不過，您的CRM可能一開始是透過重複專案傳送。 以下說明合併方法。

>[!CAUTION]
>
>合併人員是永久性的，沒有「還原」選項。

>[!PREREQUISITES]
>
>尋找及合併重複專案涉及使用[內建/系統智慧列示](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}。

>[!NOTE]
>
>Marketo不會針對[!DNL Salesforce]或[!DNL Microsoft Dynamics]同步自動進行重複資料刪除，或當您手動輸入人員時。

## 尋找重複專案 {#find-duplicates}

1. 前往「**[!UICONTROL Database]**」區域。

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >如果您使用[!DNL Salesforce]個人帳戶，在Marketo中合併人員可能無法運作。 請儘可能合併[!DNL Salesforce]中的記錄。

1. 選取&#x200B;**[!UICONTROL Possible Duplicates]**&#x200B;系統智慧清單，然後按一下&#x200B;**[!UICONTROL People]**&#x200B;標籤。

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >您也可以[找到具有自訂邏輯的重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}。

## 手動合併人員 {#merge-people-manually}

>[!CAUTION]
>
>合併人員時，如果落選者擁有Marketo自訂物件，則系統不會&#x200B;_將_&#x200B;重新關聯至成功人員。 在執行合併之前，請重新父系自訂物件。

1. 按住Ctrl/Cmd鍵並按一下，然後按一下&#x200B;**[!UICONTROL Merge People]**&#x200B;以選取重複專案。

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >您可以為同一個人員設定兩個或多個重複專案 — 一次選取所有專案。

1. 不符合的記錄之間的值會出現。 _選取您要為每個欄位保留的值_。 完成時，按一下&#x200B;**[!UICONTROL Merge]**。 如果您不想要其中一個值，可以核取&#x200B;**[!UICONTROL Custom]**&#x200B;並輸入您選擇的值。

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >* 與Salesforce不同，在Marketo中合併人員時，他們的分數是&#x200B;_而不是_&#x200B;總和。 您可以選取要保留的值。
   >
   >* 手動合併人員時，第一個選取的人員即為「獲勝者」。 所以在「人物」索引標籤中，如果您要合併記錄ID 198與199，而且剛好是先按一下199,199將會是合併之人士的記錄ID。 如果合併兩個以上的記錄，這也適用。

   >[!TIP]
   >
   >合併總比刪除好。 您將保留所有歷史記錄（頁面瀏覽次數、連結點選、電子郵件開啟、表單填寫等）。

## Salesforce中的效果 {#effect-in-salesforce}

如果您整合了Salesforce，在Salesforce中合併銷售機會的影響有幾條注意事項。

* 僅合併潛在客戶或僅合併聯絡人時，會根據一般[!DNL Salesforce]規則合併。
* 將銷售線索與聯絡人合併在一起時，所有銷售線索都會先轉換為聯絡人，再依據一般[!DNL Salesforce]規則合併。

有關合併潛在客戶或聯絡人時Salesforce行為的詳細資訊，請檢查下列[!DNL Salesforce]檔案：

* [正在合併重複的銷售機會](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&language=en_US){target="_blank"}
* [正在合併重複的連絡人](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&language=en_US){target="_blank"}

## 大量合併 {#bulk-merging}

如果您有太多重複專案需要手動合併，請聯絡Adobe客戶團隊（您的客戶經理）以討論您的選項。
