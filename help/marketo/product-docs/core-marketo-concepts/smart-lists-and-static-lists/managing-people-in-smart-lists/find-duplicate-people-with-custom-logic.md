---
unique-page-id: 2952636
description: 使用自訂邏輯尋找重複人員 — Marketo檔案 — 產品檔案
title: 使用自訂邏輯尋找重複的人員
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 0%

---

# 使用自訂邏輯尋找重複的人員 {#find-duplicate-people-with-custom-logic}

Marketo Engage具有系統智慧清單，可透過比對重複人員的電子郵件地址來尋找重複人員。 如果您想使用其他欄位來尋找與的重複專案，以下說明方式。

>[!PREREQUISITES]
>
>[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**&#x200B;區域。

![](assets/ma-2.png)

1. 選取您的智慧清單，按一下&#x200B;**[!UICONTROL Smart List]**&#x200B;標籤。

   ![](assets/two-4.png)

1. 尋找&#x200B;**[!UICONTROL Duplicate Fields]**&#x200B;篩選器並拖曳到畫布上。

   ![](assets/three-4.png)

1. 從四個可用選項中選擇一個：

   * [!UICONTROL Email Address]
   * [!UICONTROL Full Name]
   * [!UICONTROL Last Name]
   * [!UICONTROL Updated At]

   >[!NOTE]
   >
   >除「電子郵件地址」外，所有欄位都區分大小寫。 所以在[全名]欄位中使用[john doe]將&#x200B;_不會_&#x200B;傳回John Doe的結果。

   ![](assets/four-2.png)

   完成！ 執行「智慧列示」，在先前選取的欄位中尋找具有相同值的人員。
