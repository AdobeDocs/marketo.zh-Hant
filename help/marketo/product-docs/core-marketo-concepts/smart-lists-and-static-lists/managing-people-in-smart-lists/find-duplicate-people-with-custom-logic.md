---
unique-page-id: 2952636
description: 使用自訂邏輯尋找重複人員-Marketo檔案——產品檔案
title: 使用自訂邏輯尋找重複人員
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 5%

---

# 尋找具有自訂邏輯{#find-duplicate-people-with-custom-logic}的重複人員

Marketo有一個系統智慧清單，通過匹配其電子郵件地址來查找重複的人。 如果您想使用其他欄位來尋找重複項目，請參閱以下說明。

>[!PREREQUISITES]
>
>[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 前往&#x200B;**行銷活動**&#x200B;區域。

![](assets/ma-2.png)

1. 選擇智慧清單，按一下&#x200B;**智慧清單**&#x200B;頁籤。

   ![](assets/two-4.png)

1. 尋找&#x200B;**複製欄位**&#x200B;篩選器並拖曳至畫布。

   ![](assets/three-4.png)

1. 從四個可用選項中選擇一個：

   * 電子郵件地址
   * 全名
   * 姓氏
   * 更新日期：

   >[!NOTE]
   >
   >除「電子郵件地址」外，所有欄位都區分大小寫。 因此，在「全名」欄位中使用「john doe」會&#x200B;_not_&#x200B;傳回John Doe的結果。

   ![](assets/four-2.png)

   完成! 執行智慧型清單，在先前選取的欄位中尋找具有相同值的人。
