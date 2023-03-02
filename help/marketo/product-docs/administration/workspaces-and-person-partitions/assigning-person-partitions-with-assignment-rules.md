---
unique-page-id: 2360327
description: 使用指派規則指派人員分區 — Marketo檔案 — 產品檔案
title: 使用分配規則分配人員分區
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
source-git-commit: 57b94e643154b1463d9fd65295a66f1a3286fd40
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 使用分配規則分配人員分區 {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**需要管理權限**

>[!PREREQUISITES]
>
>[建立人員分區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

使用人員分區時，請設定分配規則，將從CRM建立的人員路由至其各自的分區。

>[!NOTE]
>
>只有透過CRM和SOAP API在Marketo中建立的使用者，才會套用指派規則。

1. 前往 **管理** 的上界。

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. 按一下 **工作區與分區**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. 在 **人員分區** 按一下 **分配規則**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. 按一下 **添加選擇** 添加將人員分配到人員分區的條件。

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. 選取條件應建置的欄位。

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. 選擇選擇運算子並輸入值。

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. 選擇您希望符合條件的人員進入的「人員分區」。

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >您可以視需要新增多個選項。

1. 按一下 **儲存**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

就在這！ 您已指派規則來將人員填入人員分區！

>[!NOTE]
>
>如果未滿足任何先前的條件，則將應用預設選擇。
