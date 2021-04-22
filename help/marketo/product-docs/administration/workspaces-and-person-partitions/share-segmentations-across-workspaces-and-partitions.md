---
unique-page-id: 7515767
description: 跨工作區和分區共用細分-Marketo文檔——產品文檔
title: 跨工作區和分區共用區段
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 跨工作區和分區共用分區{#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>本文僅適用於具有「工作區」和「分區」的客戶。

## 什麼是細分？{#whats-a-segmentation}

Marketo非常擅長挑選適合的人來參與計畫或明智的宣傳活動。 不過，若是較永久的角色，您應使用區段。 他們需要在Marketo使用進階的動態內容。

>[!NOTE]
>
>瞭解如何建立區段[。](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

一旦您設定好這些角色（_和_&#x200B;您使用工作區），您就會想要在整個工作區中共用這些角色。 以下是一些值得瞭解的好事：

## 規則與提示{#rules-tips}

* 每份Marketo訂閱最多可包含20個跨多個工作區的「總計」區段（每個工作區&#x200B;**不是20個**）。
* 您只能與您有權存取的工作區共用區段。
* 請務必建立並使用&#x200B;**預設工作區，該工作區可以查看所有分區**。

* 區段處理只會在建立區段的工作區中執行。

   * 在預設工作區中建立您要共用的區段。
      * 核准區段
      * 共用工作區會看到鎖定的資料夾，且區段為唯讀。
      * 無法編輯共用版本。 您只能編輯原始區段的建立位置。
   * 當您按一下共用區段中的區段（例如醫療保健）時，您所看見的人員將只是與您所檢視之工作區相關聯的分區中的人員。
      * 如果您在Workspace 1(WS1)中建立區段並與WS2共用，而WS1則無法存取WS2的區段，則不會重新計算區段。
      * 如果您在具有有限分區的工作區中建立區段，然後與另一個工作區共用，則收到共用區段的工作區只有在人員重疊時才會看見他們。


>[!NOTE]
>
>這些規則有些有些複雜。 開始使用最簡單的方式就是測試特定人員。 您隨時都可以進行新細分，並移除舊細分。

## 範例藍本{#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## 共用區段{#share-a-segmentation}

1. 轉至&#x200B;**Database**。

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. 按一下右鍵&#x200B;**分段**&#x200B;並選擇&#x200B;**新建資料夾**。

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. 為要在各工作區間共用的資料夾命名(範例：共用區段)。

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. 將您要共用的區段移至資料夾。

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. 按一下右鍵該資料夾並選擇&#x200B;**共用資料夾**。

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. 選擇要與共用資料夾的工作區。 按一下&#x200B;**保存**。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >該對話框顯示您有權查看的工作區，這就是為什麼Marketo建議從可查看所有工作區和分區的預設工作區建立和共用分段。

原始資料夾在資料庫樹中顯示，其中帶有一個箭頭，指示它已與其他工作區共用。 在共用工作區中，資料夾會顯示鎖定，以指出資料夾的內容已從其他工作區共用，且為唯讀。
