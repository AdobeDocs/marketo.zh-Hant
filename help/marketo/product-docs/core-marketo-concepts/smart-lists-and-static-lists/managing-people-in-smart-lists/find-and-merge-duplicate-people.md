---
unique-page-id: 557339
description: 查找並合併重複人員-Marketo文檔——產品文檔
title: 查找並合併重複人員
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 查找並合併重複人員{#find-and-merge-duplicate-people}

Marketo會在新人進入系統時自動消除重複。 不過，您的CRM最初可能已將復本傳送至Marketo。 以下是如何合併它們。

>[!NOTE]
>
>Marketo不會針對Salesforce或Microsoft Dynamics同步或手動輸入人員時自動消除重複資料。

>[!PREREQUISITES]
>
>查找和合併重複項將涉及使用[內置／系統智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)。

## 查找重複項{#find-duplicates}

1. 轉至&#x200B;**Database**&#x200B;區域。

   ![](assets/db.png)

   >[!CAUTION]
   >
   >如果您使用Salesforce人員帳戶，合併Marketo地區的人員可能無法運作。 請盡可能合併Salesforce中的記錄。

1. 選擇&#x200B;**Possible Duplicates**&#x200B;系統智慧清單，然後按一下&#x200B;**People**&#x200B;頁籤。

   ![](assets/two.png)

   >[!NOTE]
   >
   >您也可以[尋找具有自訂邏輯的重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md)。

## 手動合併人員{#merge-people-manually}

>[!CAUTION]
>
>合併人員時，如果失去的人有Marketo自訂物件，**not**&#x200B;將重新與獲勝的人關聯。 在執行合併之前，請重新為自訂物件建立父級。

1. 按住Ctrl/Cmd並按一下以選擇復本，然後按一下&#x200B;**合併人員**。

   ![](assets/three.png)

   >[!TIP]
   >
   >您可以為同一人提供兩個或更多重複項——一次選擇全部。

1. 您將看到&#x200B;_不符合_&#x200B;的記錄之間的值。 選擇要保留的值。 完成時，按一下&#x200B;**合併**。 如果您不需要任一值，可以檢查&#x200B;**Custom**&#x200B;並輸入您選擇的值。

   ![](assets/four.png)

   >[!NOTE]
   >
   >手動合併人員時，第一個選取的人將是「贏家」。 因此，在「人物」標籤中，如果您要合併記錄ID 198和199，而您恰好先點按199,199將會是合併者的記錄ID。 如果合併了兩個以上的記錄，也會適用這種情況。

   >[!TIP]
   >
   >合併比刪除更好。 您將保留所有歷史記錄（頁面瀏覽、連結點按、電子郵件開啟、表單填滿等）。

## 在Salesforce {#effect-in-salesforce}中的效果

如果您有Salesforce整合，則有一些關於Salesforce中合併銷售線索的效果的附註。

* 當僅合併Lead或僅合併Contact時，它們會根據常規Salesforce規則合併。
* 合併Lead和Contact時，所有Lead都會在根據常規Salesforce規則合併之前轉換為Contact。

有關合併Lead或Contact時Salesforce行為的具體資訊，請查看以下Salesforce文檔：

* [合併重複銷售線索](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [合併重複聯繫人](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## 批量合併{#bulk-merging}

如果您有太多重複項目無法手動合併，請連絡您的客戶成功經理以討論您的選項。

超級！ 如果您連線至CRM，記錄會根據下列規則合併到該處。
