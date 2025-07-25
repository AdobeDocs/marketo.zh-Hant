---
unique-page-id: 14352508
description: 建立自訂動態欄位 — Marketo檔案 — 產品檔案
title: 建立自訂動態欄位
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 建立自訂動態欄位 {#create-custom-dynamic-fields}

建立自訂動態欄位有兩個方法。

## 儲存一位或幾位連絡人的自訂欄位 {#saving-custom-fields-for-one-or-a-few-contacts}

1. 在[!UICONTROL People]頁面中按一下連絡人的名稱。

1. 選擇[!UICONTROL Unsubscribe]旁邊的下拉式清單，然後選取&#x200B;**[!UICONTROL Edit]**。

1. 向下捲動至編輯頁面底部。 然後，您可以為欄位建立名稱和值。

1. 按一下「**[!UICONTROL Save]**」。

## 正在儲存許多連絡人的自訂欄位 {#saving-custom-fields-for-many-contacts}

1. 建立CSV試算表，並在其欄位中放入自訂欄位。

1. 依照[一般CSV上傳程式](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)執行，在欄位對應畫面上停止。

1. 請從下拉式清單中選取&#x200B;**[!UICONTROL Add a new Custom Field]**，而不是其中一個預設欄位。

1. 輸入您想要的欄位名稱，然後按一下&#x200B;**[!UICONTROL OK]**。

1. 完成上傳CSV。 您的連絡人將會透過新增的自訂欄位進行輸入。

>[!NOTE]
>
>建立自訂欄位後，大約需要30分鐘該欄位才會顯示在範本編輯器的動態欄位下拉式清單中。

## 如何在範本中使用自訂欄位 {#how-to-use-your-custom-fields-in-a-template}

使用上述方法儲存自訂欄位後，您就可以在範本中參照它們。

1. [建立範本](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md)並按一下&#x200B;**[!UICONTROL Dynamic Fields]**&#x200B;按鈕，如同您一般的作法。

1. 從出現的下拉式清單中選取&#x200B;**[!UICONTROL Custom Fields]**。

1. 您會看到預先儲存的自訂欄位，並可選取一個欄位來填寫範本。
