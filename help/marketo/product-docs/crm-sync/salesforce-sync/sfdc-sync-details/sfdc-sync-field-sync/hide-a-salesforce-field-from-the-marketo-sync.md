---
unique-page-id: 4719306
description: 在行銷人員同步——行銷人員檔案——產品檔案中隱藏Salesforce欄位
title: 在Marketon Sync中隱藏Salesforce欄位
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# 在Marketon Sync中隱藏Salesforce欄位 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**需要管理員權限**

並非Salesforce中的每個欄位都對行銷有用。 您只能包含所需的欄位，以最佳化同步效能。 以下說明如何隱藏欄位，讓Marketo免受損失。

1. 按一下您的名稱功能表，然後選取「 **設定」**。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 在搜 **尋列中輸入描述檔** ，然後按一下「管理使用者」下的「描述檔 **」(Profiles** ) ****。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 按一下同步使用者的設定檔。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在「 **Field-Level Security** 」（欄位層級安全性）區段下，按一 **下包含目標欄位之物件旁的「View** 」（檢視）。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 按一 **下編輯**。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消選中 **要隱藏的欄位旁邊的** 「可見」複選框。 按一下 **儲存**。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在Salesforce中隱藏的欄位已與Marketo同步，則您也需要在Marketo中隱藏，如果您不想使用它。

   就這樣！ 下次同步完成後，您將不會再在Marketo中看到此欄位。

   >[!NOTE]
   >
   >**相關文章**
   >
   >    
   >    
   >    * [隱藏和取消隱藏欄位](../../../../../product-docs/administration/field-management/hide-and-unhide-a-field.md)


