---
unique-page-id: 4720232
description: 建立新帳戶清單 — Marketo檔案 — 產品檔案
title: 建立新的帳戶清單
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 建立新的帳戶清單 {#create-a-new-account-list}

建立並上傳組織和網域名稱清單，以透過個人化行銷活動鎖定這些關鍵帳戶。

>[!NOTE]
>
>本文僅適用舊版Web ABM客戶。 如果您在2016年9月之後取得Web ABM，請依照中的步驟進行 [本文](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) 而非。

## 建立新的帳戶清單 {#create-a-new-account-list-1}

1. 前往 **帳戶清單**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. 選取 **新建**.

   ![](assets/create-new-account-list-hand.jpg)

1. 選取 **瀏覽** 並上傳您的CSV檔案（確認csv檔案符合條件）。 新增 **名稱** 和 **說明**. 按一下 **儲存**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**CSV檔案的格式為何？**
   >
   >確定具名帳戶CSV檔案符合以下要求：
   >
   >* 已儲存為CSV格式
   >* 不超過10MB
   >* 只有4個欄位具有標題「A：名稱」、「B：網域」、「C：國家/地區」、「D：美國州」。
   >* 上傳的檔案在核准前最多可能需要2個工作天的時間。
   >* 您會收到核准電子郵件通知，或檢查「指定帳戶」頁面中的檔案狀態。
   >* 針對所有已上傳清單累計的記錄/列總數從10K開始，最大套件總計為10K。

   >[!NOTE]
   >
   >**CSV檔案的範例**
   >
   >* 資料列1欄位A值=組織
   >* 第1列第B欄值=網域
   >* 列1欄C值=國家/地區
   >* 列1欄D值=美國州別
   >* 其中一個欄值是強制的。 不過，同時提供「組織」和「網域」名稱可改善「帳戶清單」的符合率。
   >* 「國家/地區」和「州」為可選值。
   >
   >   * 若為國家/地區名稱，請使用完整的國家/地區名稱或縮寫代碼。 例如： 美國或美國。
   >   * 若為美國州別，請使用2字母縮寫代碼，即CA。 僅可辨識美國狀態。
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## 編輯帳戶清單 {#edit-an-account-list}

在 **帳戶清單** 頁面，按一下 **編輯** 圖示。

![](assets/create-new-account-list-edit.jpg)

選取 **瀏覽** 並上傳新的CSV檔案。 此檔案將取代原始檔案。 按一下 **儲存**. 新上傳的檔案將處於擱置狀態，直到Marketo支援核准為止；當處於擱置狀態時，原始檔案將保持活動狀態。

![](assets/set-account-list-edit-hands.jpg)

CSV檔案會取代現有的檔案。 在新檔案處理完成之前，現有清單將保持活動狀態。

## 刪除具名帳戶清單 {#delete-a-named-account-list}

1. 在 **帳戶清單** 頁面上，按一下要刪除之清單的「刪除」圖示。

   ![](assets/create-new-account-list-delete.jpg)

1. 系統會顯示訊息，確認您是否要刪除清單。 按一下 **確定**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[使用科目清單建立節段](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
