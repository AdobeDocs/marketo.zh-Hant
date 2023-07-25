---
unique-page-id: 2360327
description: 使用指派規則指派人員分割 — Marketo檔案 — 產品檔案
title: 使用指派規則指派人員分割
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 使用指派規則指派人員分割 {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**需要管理員許可權**

>[!PREREQUISITES]
>
>[建立個人資料分割](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

使用人員資料分割時，請設定指派規則，以將從CRM建立的人路由到其各自的分割區。

>[!NOTE]
>
>只有從CRM和透過SOAP API在Marketo中建立的人員才會套用指派規則。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. 按一下 **[!UICONTROL 工作區與分割區]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. 在 **[!UICONTROL 個人資料分割]** 標籤，按一下 **[!UICONTROL 指派規則]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. 按一下 **[!UICONTROL 新增選擇]** 新增將人員路由至人員分割區的條件。

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. 選取應建立條件的欄位。

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. 選擇選擇運運算元並輸入值。

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. 選取您想要符合條件的人所屬的「人員分割」。

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >您可以新增任意數量的選擇。

1. 按一下 **[!UICONTROL 儲存]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

而且您已經擁有了！ 您已指派規則來填入人員分割區！

>[!NOTE]
>
>如果不符合先前的任何條件，則會套用「預設選擇」。
