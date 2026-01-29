---
unique-page-id: 2360309
description: 了解工作區和人員分割 — Marketo 文件 — 產品文件
title: 了解工作區和人員分割
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '528'
ht-degree: 100%

---

# 了解工作區和人員分割 {#understanding-workspaces-and-person-partitions}

## 工作區 {#workspaces}

>[!CAUTION]
>
>工作區的設定方式可能很複雜。請和 [Marketo 支援](https://nation.marketo.com/t5/Support/ct-p/Support)聯絡，以了解其是否適合您。

工作區是在 Marketo 中保存行銷資產的獨立區域，例如計畫、登陸頁面、電子郵件等。其可供多人使用。每個使用者都可存取一或多個工作區。

>[!NOTE]
>
>**範例**
>
>您可能會使用工作區的部分原因：
>
>* 地理位置：歐洲、亞洲和北美洲的行銷部門各有專屬工作區
>* 業務單位：[!DNL Quicken]、[!DNL Quickbooks] 和 [!DNL TurboTax] 各有專屬工作區
>
>在每種情況下，分隔的原因是因為行銷資產完全不同。如果其可共用行銷資產，則工作區可能就並非適合您使用的工具。

>[!NOTE]
>
>了解如何建立[建立新工作區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md)。

## 跨工作區共用 {#sharing-across-workspaces}

以下說明如何在工作區之間共用資產。無論您想要共用什麼，運作方式都一樣；此範例則展示分段。

>[!NOTE]
>
>包含您資產的上層資料夾是唯一可共用的資料夾，下層資料夾則無法共用。

1. 按一下「**[!UICONTROL Database]**」。

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. 在「分段」資料夾上按一下滑鼠右鍵，然後按一下 **[!UICONTROL New Folder]**。

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. 為資料夾命名，然後按一下 **[!UICONTROL Create]**。

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. 將您想要共用的資產移至資料夾。

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. 以滑鼠右鍵按一下資料夾，然後選取 **[!UICONTROL Share Folder]**。

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. 選取您想要共用該資料夾的工作區，然後按一下 **[!UICONTROL Save]**。「共用資料夾」對話框只會顯示您擁有檢視權限的工作區。

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >原始資料夾現在會出現一個小綠色箭頭，表示它已被共用。在已共用的工作區中，資料夾會出現表示唯讀的掛鎖。

您可以跨工作區共用這些項目。

* 電子郵件範本
* 登陸頁面範本
* 模型
* 智慧行銷活動
* [智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [分段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 程式碼片段

## 跨工作區原地複製 {#cloning-across-workspaces}

對於非範本的資產，最好在方案內部將其原地複製為本機資產。具有適當的存取層級後，您即可將這些資產拖放至另一個工作區：

* 方案
* 電子郵件
* 登陸頁面
* 表單

>[!IMPORTANT]
>
>雖然上述所有項目都可以跨工作區進行原地複製，但在原地複製時，_都必須在方案內_。

>[!NOTE]
>
>原地複製具有範本的資產時，必須先將這些範本和目的地工作區共用。

## 將資產搬移至其他工作區 {#moving-assets-to-other-workspaces}

若要將資產搬移至新的工作區，請將資產放入資料夾，然後將該資料夾拖曳至其他工作區。

>[!NOTE]
>
>您無法將包含成員的方案從一個工作區搬移到另一個工作區。

## 人員分割 {#person-partitions}

人員分割的功用類似於獨立的資料庫。每個分割都具有自己的人員，不會去除重複或與其他分割混合。如果您認為您的商務使用案例可能需要使用相同電子郵件地址的重複記錄，請和 [Marketo 支援](https://nation.marketo.com/t5/Support/ct-p/Support)聯絡。

您可以指派人員分割至下列設定中的[工作區](create-a-new-workspace.md)：

* 一個工作區對一個人員分割 (1:1)
* 一個工作區對多個人員分割 (1:x)
* 多個工作區對一個人員分割 (x:1)

>[!NOTE]
>
>您會使用人員分割的原因：
>
>* 您的工作區不僅具有不同的資產，而且未共用任何人員
>* 由於其他商務原因而需要重複項目

>[!CAUTION]
>
>人員分割相互獨立、不會互動，因此在設定時需特別小心。

>[!NOTE]
>
>了解如何[建立人員分割](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)。
