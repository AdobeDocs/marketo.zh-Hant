---
unique-page-id: 4719306
description: 在「Marketo同步-Marketo文檔——產品文檔」中隱藏Salesforce欄位
title: 在Marketo同步中隱藏Salesforce欄位
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# 在Marketo同步{#hide-a-salesforce-field-from-the-marketo-sync}中隱藏Salesforce欄位

>[!NOTE]
>
>**需要管理員權限**

並非Salesforce中的每個欄位都對行銷有用。 您只能包含所需的欄位，以最佳化同步效能。 這樣你就能躲開Marketo。

1. 按一下您的名稱菜單，然後選擇&#x200B;**Setup**。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 在搜索欄中輸入&#x200B;**profiles** ，然後按一下&#x200B;**管理用戶**&#x200B;下的&#x200B;**Profiles**。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 按一下同步使用者的設定檔。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在&#x200B;**Field-Level Security**&#x200B;區段下，按一下包含目標欄位之物件旁的&#x200B;**View**。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 按一下&#x200B;**編輯**。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消選中要隱藏的欄位旁邊的&#x200B;**Visible**&#x200B;複選框。 按一下&#x200B;**保存**。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在Salesforce中隱藏的欄位已與Marketo同步，您也需要在Marketo隱藏，如果您不想使用它。

   就這樣！ 下次同步完成後，您將不再在Marketo看到此欄位。

   >[!MORELIKETHIS]
   >
   >[隱藏和取消隱藏欄位](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
