---
unique-page-id: 2360327
description: 使用分配規則分配人員分區-Marketo文檔——產品文檔
title: 使用分配規則分配人員分區
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# 使用分配規則{#assigning-person-partitions-with-assignment-rules}分配人員分區

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>[建立人員分區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

使用人員分區時，請設定分配規則，將從CRM建立的人員路由到其各自的分區。

>[!NOTE]
>
>只有在Marketo從您的CRM和透過SOAP API建立的人員，才會套用指派規則。

1. 在「管理」下，按一下「工作區與分區」。

   ![](assets/image2014-9-17-10-3a32-3a55.png)

1. 在&#x200B;**人員分區**&#x200B;頁籤下，按一下&#x200B;**分配規則**。

   ![](assets/two-6.png)

1. 按一下&#x200B;**添加選擇**&#x200B;添加條件，將人員路由到人員分區。

   ![](assets/three-6.png)

1. 選擇應建立條件的欄位。

   ![](assets/four-5.png)

1. 選擇選擇運算子並輸入值。

   ![](assets/five-1.png)

1. 選擇您希望符合條件的人員落入的人員分區。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >您可以視需要新增多種選擇。

1. 按一下&#x200B;**保存**。

   ![](assets/seven.png)

就這樣！ 您已指派規則，將人員分區填入人員！

>[!NOTE]
>
>如果未符合任何先前的條件，則會套用預設選擇。
