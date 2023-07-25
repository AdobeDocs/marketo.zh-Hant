---
unique-page-id: 557339
description: 尋找及合併重複人員 — Marketo檔案 — 產品檔案
title: 尋找並合併重複人員
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 尋找並合併重複人員 {#find-and-merge-duplicate-people}

當有新人員進入系統時，Marketo會自動刪除重複專案。 不過，您的CRM一開始可能會傳送重複資料給Marketo。 以下說明合併方法。

>[!CAUTION]
>
>合併人員是永久性的，沒有「還原」選項。

>[!PREREQUISITES]
>
>尋找及合併重複專案將使用下列專案： [內建/系統智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo不會針對Salesforce或Microsoft Dynamics同步處理或手動輸入人員時自動進行重複資料刪除。

## 尋找重複專案 {#find-duplicates}

1. 前往 **資料庫** 區域。

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >如果您使用Salesforce人員帳戶，在Marketo中合併人員可能無法運作。 如有可能，請合併Salesforce中的記錄。

1. 選取 **可能的重複專案** 系統智慧清單，然後按一下 **人員** 標籤。

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >您也可以 [使用自訂邏輯尋找重複的人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## 手動合併人員 {#merge-people-manually}

>[!CAUTION]
>
>合併人員時，如果落選人員有Marketo自訂物件，則會 **not** 重新與成功者建立關聯。 在執行合併之前，請重新為自訂物件加上父系。

1. 按住Ctrl/Cmd鍵並按一下，然後按一下 **合併人員**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >您可以為同一個人員設定兩個或多個重複專案 — 一次選取所有專案。

1. 您將看到以下記錄之間的值： _不要_ 相符。 為每個欄位選取要保留的值。 按一下 **合併** 完成時。 如果您不想要其中一個值，可以核取 **自訂** 並輸入您選擇的值。

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >手動合併人員時，第一個選取的人員將會是「獲勝者」。 因此，在「人物」索引標籤中，如果您合併記錄ID 198和199，而且碰巧先按一下199,199將是合併之人的記錄ID。 如果合併兩個以上的記錄，這也適用。

   >[!TIP]
   >
   >合併總比刪除好。 您將保留所有歷史記錄（頁面瀏覽次數、連結點選、電子郵件開啟、表單填寫等）。

## Salesforce中的效果 {#effect-in-salesforce}

如果您有Salesforce整合，有一些關於在Salesforce中合併銷售機會的效果的附註。

* 僅合併潛在客戶或僅合併聯絡人時，會根據一般Salesforce規則合併。
* 當合併銷售線索與聯絡人時，所有銷售線索都會先轉換為聯絡人，再依據一般Salesforce規則合併。

有關合併Lead或Contact時Salesforce行為的詳細資訊，請檢視以下Salesforce檔案：

* [合併重複的銷售機會](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US){target="_blank"}
* [合併重複的連絡人](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US){target="_blank"}

## 大量合併 {#bulk-merging}

如果您有太多要手動合併的重複專案，請聯絡Adobe客戶團隊（您的客戶經理）以討論您的選項。
