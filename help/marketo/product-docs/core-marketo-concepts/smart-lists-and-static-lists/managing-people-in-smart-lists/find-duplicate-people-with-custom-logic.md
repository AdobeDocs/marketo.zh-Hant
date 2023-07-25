---
unique-page-id: 2952636
description: 使用自訂邏輯尋找重複人員 — Marketo檔案 — 產品檔案
title: 使用自訂邏輯尋找重複的人員
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# 使用自訂邏輯尋找重複的人員 {#find-duplicate-people-with-custom-logic}

Marketo有一個系統智慧清單，可透過比對重複人員的電子郵件地址來尋找重複人員。 如果您想使用其他欄位來尋找重複專案，請參閱以下方法。

>[!PREREQUISITES]
>
>[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 前往 **行銷活動** 區域。

![](assets/ma-2.png)

1. 選取您的智慧清單，按一下 **智慧清單** 標籤。

   ![](assets/two-4.png)

1. 尋找並拖曳 **重複欄位** 篩選至畫布上。

   ![](assets/three-4.png)

1. 從四個可用選項中選擇一個：

   * 電子郵件地址
   * 全名
   * 姓氏
   * 更新時間

   >[!NOTE]
   >
   >除「電子郵件地址」外，所有欄位都區分大小寫。 因此，在「全名」欄位中使用「john doe」將 _not_ 傳回John Doe的結果

   ![](assets/four-2.png)

   完成! 執行智慧清單，以尋找在先前選取的欄位中具有相同值的使用者。
