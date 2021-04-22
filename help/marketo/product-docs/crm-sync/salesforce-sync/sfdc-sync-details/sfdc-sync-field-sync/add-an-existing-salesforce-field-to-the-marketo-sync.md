---
unique-page-id: 4719308
description: 將現有的Salesforce欄位新增至Marketo同步-Marketo檔案——產品檔案
title: 將現有的Salesforce欄位新增至Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 將現有的Salesforce欄位新增至Marketo同步{#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理員權限**

通常，Salesforce中的新自訂欄位會自動同步至Marketo。 否則，Marketo同步用戶可能看不到這些欄位。 這就是您如何修正的。

1. 按一下您的名稱，然後選擇&#x200B;**Setup**。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 在左搜索欄中輸入&#x200B;**profile** ，然後按一下&#x200B;**Manage Users**&#x200B;下的&#x200B;**Profiles**。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. 按一下同步使用者的設定檔。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. 在&#x200B;**Field-Level Security**&#x200B;區段下，按一下包含該欄位的對象旁的&#x200B;**View**。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 按一下&#x200B;**編輯**。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 選中要添加到同步的欄位的&#x200B;**Visible**&#x200B;複選框，然後按一下&#x200B;**Save**。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   真貼心！ 在下一個同步週期，Marketo將看到這個場並啟動魔法。

   >[!NOTE]
   >
   > 如果欄位在Salesforce中已有值，則這些值要等到下次記錄更新時才會同步至Marketo。
