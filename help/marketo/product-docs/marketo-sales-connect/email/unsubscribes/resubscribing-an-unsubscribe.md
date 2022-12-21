---
unique-page-id: 14746177
description: 重新訂閱取消訂閱 — Marketo檔案 — 產品檔案
title: 重新訂閱取消訂閱
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 重新訂閱取消訂閱 {#resubscribing-an-unsubscribe}

有時候，人們會想要選擇回收電子郵件。 以下說明如何讓取消訂閱可再次傳送。

>[!NOTE]
>
>**需要管理權限**

>[!CAUTION]
>
>在重新訂閱某人之前，您應該能夠證明重新訂閱該人的授權是有檔案記錄的，並且符合所有適用法律。

>[!NOTE]
>
>如果已開啟「取消訂閱同步」，則必須從ToutApp中刪除取消訂閱，並取消選中Salesforce中的選擇退出，以使人員記錄不再同步。

1. 前往 [網頁應用程式](https://toutapp.com/login) 按一下 **人員**.

1. 選擇要開啟人員詳細資訊視圖的人員。

   ![](assets/two.png)

1. 在「人員詳細資訊」檢視中按一下三個點，然後選取 **移除取消訂閱**.

   ![](assets/three.png)

1. 選取人員被選擇回收電子郵件的原因，然後按一下 **移除取消訂閱**.

   ![](assets/four.png)

>[!NOTE]
>
>如果您已開啟「取消訂閱同步」，則必須同時取消選中Salesforce中記錄上的選擇退出框，否則夜間同步將重新取消訂閱Sales Connect中的人員，因為它將檢測該人員在Salesforce中已選擇退出。 如果其中一個記錄選擇退出/取消訂閱，同步會將連結的記錄標示為此類記錄。
