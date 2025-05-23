---
unique-page-id: 2360309
description: 瞭解工作區和人員分割 — Marketo檔案 — 產品檔案
title: 瞭解工作區和人員分割
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 91b6460bf0fa7fed85d48887ec38203f2ee7440f
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 瞭解工作區和人員分割 {#understanding-workspaces-and-person-partitions}

## 工作區 {#workspaces}

>[!CAUTION]
>
>工作區可能設定起來很複雜。 請連絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)，瞭解他們是否適合您。

工作區是Marketo中存放行銷資產的獨立區域，例如方案、登陸頁面、電子郵件等。 可供多人使用。 每個使用者都可存取一或多個工作區。

>[!NOTE]
>
>**範例**
>
>您可以使用工作區的部分原因：
>
>* 地理位置：歐洲、亞洲和北美的行銷部門各有專屬的工作區
>* 業務單位： [!DNL Quicken]、[!DNL Quickbooks]和[!DNL TurboTax]各自取得工作區
>
>在每個案例中，分開是因為行銷資產完全不同。 如果他們共用行銷資產，工作區可能不是適合您的工具。

>[!NOTE]
>
>瞭解如何建立[新的工作區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md)。

## 跨工作區共用 {#sharing-across-workspaces}

以下說明如何在工作區之間共用資產。 這對您想要共用的任何專案都一樣運作；此範例顯示區段。

>[!NOTE]
>
>包含您資產的父資料夾是唯一可共用的資料夾，而非子資料夾。

1. 按一下&#x200B;**[!UICONTROL 資料庫]**。

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. 在Segmentation資料夾上按一下滑鼠右鍵，然後按一下&#x200B;**[!UICONTROL 新增資料夾]**。

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. 為資料夾命名，然後按一下[建立]。**&#x200B;**

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. 將您要共用的資產移至資料夾。

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. 在資料夾上按一下滑鼠右鍵，然後選取&#x200B;**[!UICONTROL 共用資料夾]**。

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. 選取您要共用資料夾的工作區，然後按一下[儲存]。**&#x200B;** 「共用資料夾」對話方塊只會顯示您有檢視許可權的工作區。

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >原始資料夾現在會有一個小綠色箭頭，表示它已被共用。 在共用工作區中，資料夾將具有掛鎖，表示唯讀。

您可以跨工作區共用這些專案。

* 電子郵件範本
* 登入頁面範本
* 模型
* 智慧型行銷活動
* [智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [區段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 代碼片段

## 跨工作區複製 {#cloning-across-workspaces}

對於非範本的資產，最好在程式內將其復製為本機資產。 有了適當的存取層級，您可以將這些資產拖放至另一個工作區：

* 計畫
* 電子郵件
* 登陸頁面
* Forms

>[!IMPORTANT]
>
>雖然上述所有專案都可以跨工作區複製，但複製時，_必須位於程式_&#x200B;內。

>[!NOTE]
>
>複製含有範本的資產時，這些範本必須和目的地工作區共用。

## 將Assets移至其他工作區 {#moving-assets-to-other-workspaces}

若要將資產移至新的工作區，請將資產放入資料夾，然後將資料夾拖曳至其他工作區。

>[!NOTE]
>
>您無法將包含成員的方案從一個工作區移動到另一個工作區。

## 人員分割 {#person-partitions}

個人資料分割的作用就像個別的資料庫。 每個分割區都有各自的人員，不會進行重複資料刪除或與其他分割區混合。 如果您認為您的業務使用案例可能需要具有相同電子郵件地址的重複記錄，請聯絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。

您可以指派人員分割至下列組態中的[工作區](create-a-new-workspace.md)：

* 一個工作區對一個人分割(1:1)
* 一個工作區對多個人員分割(1：x)
* 將多個工作區分割為單一人員分割(x：1)

>[!NOTE]
>
>您使用人員分割的原因：
>
>* 您的工作區不僅有不同的資產，而且未共用任何人員
>* 由於其他業務原因需要重複專案

>[!CAUTION]
>
>人員資料分割不會相互互動，因此在設定時請務必小心。

>[!NOTE]
>
>瞭解如何[建立人員資料分割](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)。
