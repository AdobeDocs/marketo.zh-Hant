---
unique-page-id: 4720232
description: 建立新帳戶清單 — Marketo檔案 — 產品檔案
title: 建立新帳戶清單
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 建立新帳戶清單 {#create-a-new-account-list}

建立並上傳組織和網域名稱清單，透過個人化行銷活動鎖定這些重要帳戶。

>[!NOTE]
>
>本文僅適用舊版Web ABM客戶。 如果您在2016年9月之後獲得了Web ABM，請按照 [這篇文章](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) 。

## 建立新帳戶清單 {#create-a-new-account-list-1}

1. 前往 **帳戶清單**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. 選擇 **新建**.

   ![](assets/create-new-account-list-hand.jpg)

1. 選擇 **瀏覽** 上傳您的CSV檔案（確認csv檔案符合條件）。 新增 **名稱** 和 **說明**. 按一下 **儲存**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**CSV檔案的格式為何？**
   >
   >確認指定的帳戶CSV檔案符合下列要求：
   >
   >* 儲存為CSV格式
   >* 不超過10MB
   >* 標題為A的僅4欄：名稱，欄B:域，列C:國家/地區，D欄：美國各州。
   >* 上傳的檔案最多需要2個工作天才能完成核准。
   >* 您會在「指定帳戶」頁面中收到核准電子郵件通知或檢查檔案狀態。
   >* 所有已上載清單的記錄/行累積總數為10K，其中最大的包總計為100K。


   >[!NOTE]
   >
   >**CSV檔案範例**
   >
   >* 行1列A值=組織
   >* 行1列B值=域
   >* 行1列C值=國家/地區
   >* 行1列D值=美國州
   >* 其中一個欄值是必填的。 不過，同時提供組織和網域名稱可改善帳戶清單的匹配率。
   >* 「國家/地區」和「國家/地區」是選用值。
      >
      >   * 對於國家/地區名稱，請使用完整的國家/地區名稱或縮寫代碼。 例如 美國或美國。
      >   * 若為美國州，請使用2個字母的縮寫代碼，即CA。 只有美國各州得到承認。

   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## 編輯帳戶清單 {#edit-an-account-list}

在 **帳戶清單** 頁面，按一下 **編輯** 表徵圖。

![](assets/create-new-account-list-edit.jpg)

選擇 **瀏覽** 並上傳新的CSV檔案。 此檔案將替換原始檔案。 按一下 **儲存**. 新上傳的檔案將處於擱置狀態，直到Marketo支援核准為止，當處於擱置狀態時，原始檔案將保持作用中狀態。

![](assets/set-account-list-edit-hands.jpg)

CSV檔案將取代現有檔案。 在新檔案的處理完成之前，現有清單會保持作用中狀態。

## 刪除指定帳戶清單 {#delete-a-named-account-list}

1. 在 **帳戶清單** 頁面，按一下您要刪除的清單的「刪除」圖示。

   ![](assets/create-new-account-list-delete.jpg)

1. 系統會顯示訊息以確認您是否要刪除清單。 按一下 **確定**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[使用帳戶清單建立區段](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
