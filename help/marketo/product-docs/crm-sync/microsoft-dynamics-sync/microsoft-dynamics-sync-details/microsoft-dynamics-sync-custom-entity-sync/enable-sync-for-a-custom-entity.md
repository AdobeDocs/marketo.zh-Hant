---
unique-page-id: 2953384
description: 啟用自訂實體的同步-Marketo檔案——產品檔案
title: 為自訂實體啟用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# 啟用自訂實體{#enable-sync-for-a-custom-entity}的同步

如果您需要Dynamics的自訂實體資料才能在Marketo使用，以下說明如何為其啟用同步：

>[!NOTE]
>
>**需要管理員權限**

>[!NOTE]
>
>當您為自訂實體啟用同步時，Marketo會執行初始同步，以匯入自訂物件的所有資料。

1. 前往&#x200B;**Admin**&#x200B;區段。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 選擇&#x200B;**Microsoft Dynamics**，然後按一下&#x200B;**禁用同步**。

   您必須暫時停用全域同步，才能啟用或停用自訂實體。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. 在「資料庫管理」下，按一下&#x200B;**Dynamics Entities Sync**&#x200B;連結。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 按一下&#x200B;**同步模式**&#x200B;連結。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. 選擇要同步的實體，然後按一下&#x200B;**啟用同步**。

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. 選擇要同步的欄位，或在智慧清單中作為[constraints](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)和／或觸發器使用。 完成後，按一下「啟用同步」。****

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >在同步過程中，您可能會注意到「動態實體同步」項目從導覽樹狀結構消失。 這是預期的行為，同步完成後將重新出現。

1. 實體現在有綠色核取標籤。

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. 別忘了重新啟用全域同步！

   ![](assets/image2015-11-10-9-3a48-3a35.png)

是啊！ 強大的功能。
