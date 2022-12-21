---
unique-page-id: 2360309
description: 了解工作區與人員分區 — Marketo檔案 — 產品檔案
title: 了解工作區和人員分區
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 了解工作區和人員分區 {#understanding-workspaces-and-person-partitions}

## 工作區 {#workspaces}

>[!CAUTION]
>
>工作區可能會很複雜而難以設定。 連絡人 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support) 找出他們是否適合你。

工作區是Marketo中個別的區域，可存放方案、登陸頁面、電子郵件等行銷資產。 可供多人使用。 每個使用者都可存取一或多個工作區。

>[!NOTE]
>
>**範例**
>
>使用工作區的一些原因：
>
>* 地理位置：歐洲、亞洲和北美市場部門各有一個工作區
>* 業務單位：Quicken、Quickbook和TurboTax各有一個工作區
>
>在每種情況下，區隔都是因為行銷資產完全不同。 如果他們共用行銷資產，則工作區可能不是適合您的工具。

>[!NOTE]
>
>了解如何建立 [建立新工作區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## 跨工作區共用 {#sharing-across-workspaces}

以下說明如何跨工作區共用資產。 對於您要共用的任何項目，它都是一樣的；此範例顯示區段。

>[!NOTE]
>
>包含您資產的父資料夾是唯一可共用的資料夾，而非子資料夾。

1. 建立新資料夾。

   ![](assets/one.png)

1. 為要共用的資料夾命名。

   ![](assets/two.png)

1. 將您要共用的資產移至資料夾。

   ![](assets/three.png)

1. 以滑鼠右鍵按一下資料夾並選取 **共用資料夾**.

   ![](assets/four.png)

1. 選擇要與共用資料夾的工作區，然後按一下 **儲存**. 「共用資料夾」(Share Folder)對話框將僅顯示您有權查看的工作區。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >原始資料夾現在會有一個綠色箭頭，表示已共用。 在共用的工作區中，資料夾會有掛鎖，表示為唯讀。

您可以在各工作區間共用這些項目。

* 電子郵件範本
* 登錄頁面範本
* 模型
* 智慧型行銷活動
* [智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [區段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 程式碼片段

## 跨工作區複製 {#cloning-across-workspaces}

若為非範本的資產，最好將其複製為程式內的本機資產。  透過適當的存取層級，您可以將這些資產拖放至另一個工作區：

* 方案
* 電子郵件
* 登錄頁面
* Forms

>[!NOTE]
>
>複製具有範本的資產時，必須與目的地工作區共用這些範本。

## 將資產移動至其他工作區 {#moving-assets-to-other-workspaces}

若要將資產移至新工作區，請將資產放入資料夾，然後將資料夾拖曳至其他工作區。

>[!NOTE]
>
>無法將包含成員的程式從一個工作區移動到另一個工作區。

## 人員分區 {#person-partitions}

人員分區的作用與單獨的資料庫類似。 每個分區都有自己的人員，他們不會刪除重複資料或與其他分區混合。 如果您認為您有業務使用案例，可能需要有具有相同電子郵件地址的重複記錄，請聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).

您可以將人員分區分配給  [工作區](create-a-new-workspace.md) 在下列設定中：

* 一個工作區對一人分區(1:1)
* 一個工作區對多人分區(1:x)
* 將多個工作區轉換為一個人員分區(x:1)

>[!NOTE]
>
>使用人員分區的原因：
>
>* 您的工作區不僅具有不同的資產，也不會共用任何人員
>* 您希望重複的項目是出於其他業務原因


>[!CAUTION]
>
>人員分區不會彼此互動，因此在設定時請小心。

>[!NOTE]
>
>了解如何 [建立人員分區](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
