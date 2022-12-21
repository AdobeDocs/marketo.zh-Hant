---
unique-page-id: 2952636
description: 使用自訂邏輯尋找重複人員 — Marketo檔案 — 產品檔案
title: 使用自訂邏輯尋找重複人員
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 5%

---

# 使用自訂邏輯尋找重複人員 {#find-duplicate-people-with-custom-logic}

Marketo有一個系統智慧清單，可比對其電子郵件地址來尋找重複的人員。 如果您想使用其他欄位來尋找重複項目，以下說明方法。

>[!PREREQUISITES]
>
>[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 前往 **行銷活動** 的上界。

![](assets/ma-2.png)

1. 選取您的智慧清單，按一下 **智慧清單** 標籤。

   ![](assets/two-4.png)

1. 尋找並拖曳 **複製欄位** 篩選至畫布。

   ![](assets/three-4.png)

1. 從四個可用選項中選擇一個：

   * 電子郵件地址
   * 全名
   * 姓氏
   * 更新日期：

   >[!NOTE]
   >
   >所有欄位（電子郵件地址除外）都區分大小寫。 所以在「全名」欄位中使用「無名氏」 _not_ 傳回無名氏的結果。

   ![](assets/four-2.png)

   完成! 執行智慧清單，在先前選取的欄位中尋找具有相同值的人員。
