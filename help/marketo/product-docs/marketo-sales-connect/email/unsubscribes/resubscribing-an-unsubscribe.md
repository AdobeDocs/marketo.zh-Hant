---
unique-page-id: 14746177
description: 重新訂閱並取消訂閱 — Marketo檔案 — 產品檔案
title: 重新訂閱取消訂閱
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 重新訂閱[!UICONTROL Unsubscribe] {#resubscribing-an-unsubscribe}

有時候，人們會想要選擇重新接收電子郵件。 以下說明如何再次將取消訂閱設為可郵寄功能。

>[!NOTE]
>
>**需要管理員許可權**

>[!CAUTION]
>
>在重新訂閱某個人之前，您應該能夠證明重新訂閱他們的授權已記錄在案，並符合所有適用法律。

>[!NOTE]
>
>如果已開啟取消訂閱同步，您必須從ToutApp移除取消訂閱，並在[!DNL Salesforce]中取消核取退出選項，讓人員記錄不再同步。

1. 移至[網頁應用程式](https://toutapp.com/login)並按一下&#x200B;**[!UICONTROL People]**。

1. 選取人員，以開啟人員詳細資料檢視。

   ![](assets/two.png)

1. 按一下人員詳細資料檢視中的三個點，然後選取&#x200B;**[!UICONTROL Remove Unsubscribe]**。

   ![](assets/three.png)

1. 選取人員選擇重新加入以接收電子郵件的原因，然後按一下&#x200B;**[!UICONTROL Remove Unsubscribe]**。

   ![](assets/four.png)

>[!NOTE]
>
>如果您開啟取消訂閱同步處理，您也必須在Salesforce中取消勾選記錄上的選擇退出方塊，或夜間同步處理會在[!DNL Sales Connect]中重新取消訂閱該人員，因為它會在[!DNL Salesforce]中偵測到該人員已選擇退出。 如果其中一個記錄選擇退出/取消訂閱，同步會將連結的記錄標籤為這樣。
