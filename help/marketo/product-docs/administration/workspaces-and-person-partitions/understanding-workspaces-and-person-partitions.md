---
unique-page-id: 2360309
description: 瞭解工作區和人員資料分割 — Marketo檔案 — 產品檔案
title: 瞭解工作區和人員資料分割
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
source-git-commit: 2d28d4b473815952231356691b1e9310c61a20f1
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# 瞭解工作區和人員資料分割 {#understanding-workspaces-and-person-partitions}

## 工作區 {#workspaces}

>[!CAUTION]
>
>工作區可能設定起來很複雜。 連絡人 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support) 以找出他們是否適合您。

工作區是Marketo中不同的區域，其中包含行銷資產，例如方案、登陸頁面、電子郵件等。 可供多人使用。 每位使用者都可存取一或多個工作區。

>[!NOTE]
>
>**範例**
>
>您可能使用工作區的部分原因：
>
>* 地理位置：歐洲、亞洲和北美的行銷部門各有專屬的工作區
>* 業務單位： [!DNL Quicken]， [!DNL Quickbooks] 和 [!DNL TurboTax] 每個都取得工作區
>
>在每個案例中，分離都是因為行銷資產完全不同。 如果他們共用行銷資產，則工作區可能不是適合您的工具。

>[!NOTE]
>
>瞭解如何建立 [建立新工作區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## 跨工作區共用 {#sharing-across-workspaces}

以下說明如何在工作區之間共用資產。 它對於您要共用的任何專案都一樣運作；此範例顯示區段。

>[!NOTE]
>
>包含您的資產的父資料夾是唯一可共用的資料夾，而非子資料夾。

1. 按一下 **[!UICONTROL 資料庫]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. 以滑鼠右鍵按一下Segmentation資料夾，然後按一下 **[!UICONTROL 新增資料夾]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. 為資料夾命名，然後按一下 **[!UICONTROL 建立]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. 將您要共用的資產移至資料夾。

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. 以滑鼠右鍵按一下資料夾，然後選取 **[!UICONTROL 共用資料夾]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. 選取您要共用資料夾的工作區，然後按一下 **[!UICONTROL 儲存]**. 「共用資料夾」對話方塊只會顯示您有檢視許可權的工作區。

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >原始資料夾現在會有一個小綠色箭頭，表示它已被共用。 在共用工作區中，資料夾將具有掛鎖，表示唯讀。

您可以跨工作區共用這些專案。

* 電子郵件範本
* 登陸頁面範本
* 模型
* 智慧型行銷活動
* [智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [區段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 代碼片段

## 跨工作區複製 {#cloning-across-workspaces}

對於非範本的資產，最好在程式內將其復製為本機資產。  使用適當的存取層級，您可以將這些資產拖放至另一個工作區：

* 計畫
* 電子郵件
* 登陸頁面
* Forms

>[!NOTE]
>
>複製含有範本的資產時，這些範本必須與目的地工作區共用。

## 將資產移至其他工作區 {#moving-assets-to-other-workspaces}

若要將資產移動到新工作區，請將資產放入資料夾，然後將資料夾拖曳到其他工作區。

>[!NOTE]
>
>您無法將包含成員的方案從一個工作區移動到另一個工作區。

## 個人資料分割 {#person-partitions}

個人資料分割就像個別的資料庫。 每個分割區都有各自的人員，不會進行重複資料刪除或與其他分割區混合。 如果您覺得有業務使用案例，需要以相同的電子郵件地址取得重複的記錄，請聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).

您可以將個人資料分割指派給  [工作區](create-a-new-workspace.md) 在下列設定中：

* 一個工作區對一個人分割(1:1)
* 一個工作區對多個人員分割(1：x)
* 多個工作區至一人分割(x：1)

>[!NOTE]
>
>您使用人員分割的原因：
>
>* 您的工作區不僅有不同的資產，而且未共用任何人員
>* 由於其他業務原因，您想要重複專案

>[!CAUTION]
>
>人員資料分割不會彼此互動，因此在設定時請務必小心。

>[!NOTE]
>
>瞭解如何 [建立人員分割](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
