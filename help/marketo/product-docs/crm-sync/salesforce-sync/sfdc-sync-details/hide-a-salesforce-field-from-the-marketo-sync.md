---
unique-page-id: 4719306
description: 從Marketo同步隱藏Salesforce欄位 — Marketo檔案 — 產品檔案
title: 從Marketo同步隱藏Salesforce欄位
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# 從Marketo同步隱藏Salesforce欄位 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**需要管理員許可權**

Salesforce並非每個欄位都適合用於行銷。 您可以僅包含您需要的欄位，以最佳化同步效能。 以下說明如何從Marketo隱藏欄位。

1. 按一下您的名稱功能表並選取 **設定**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 輸入 **設定檔** ，然後按一下 **設定檔** 在 **管理使用者**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 按一下同步處理使用者的設定檔。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在 **欄位層級安全性** 區段，按一下 **檢視** 下一個是包含目標欄位的物件。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 按一下 **編輯**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消核取 **可見** 核取方塊位於您要隱藏的欄位旁。 按一下 **儲存**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在Salesforce中隱藏的欄位已與Marketo同步，您若不想使用，也需要在Marketo中隱藏該欄位。

   完成了！ 下次同步完成後，您將無法在Marketo中看到此欄位。

   >[!MORELIKETHIS]
   >
   >[隱藏和取消隱藏欄位](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
