---
unique-page-id: 4719306
description: 隱藏Salesforce欄位，不顯示Marketo同步 — Marketo檔案 — 產品檔案
title: 隱藏Salesforce欄位，使其不受Marketo同步
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# 隱藏Salesforce欄位，使其不受Marketo同步 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**需要管理權限**

並非Salesforce中的每個欄位都對行銷有用。 您只能包含所需的欄位，以最佳化同步效能。 以下是如何隱藏欄位，不讓Marketo看到。

1. 按一下您的名稱功能表，然後選取 **設定**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 輸入 **設定檔** 在搜尋列中按一下 **設定檔** 在 **管理使用者**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 按一下同步使用者的設定檔。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在 **欄位層級安全性** ，按一下 **檢視** 位於包含目標欄位的物件旁。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 按一下 **編輯**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消核取 **可見** 要隱藏的欄位旁的核取方塊。 按一下 **儲存**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在Salesforce中隱藏的欄位已與Marketo同步，則您也需要在Marketo中隱藏，如果您不想使用它。

   就這樣！ 下次同步完成後，您將不再在Marketo中看到此欄位。

   >[!MORELIKETHIS]
   >
   >[隱藏和取消隱藏欄位](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
