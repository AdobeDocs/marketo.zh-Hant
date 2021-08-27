---
unique-page-id: 4719308
description: 將現有的Salesforce欄位新增至Marketo同步 — Marketo檔案 — 產品檔案
title: 將現有的Salesforce欄位新增至Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 將現有的Salesforce欄位新增至Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理權限**

通常，Salesforce中的新自訂欄位會自動同步至Marketo。 否則，Marketo同步使用者可能看不到這些欄位。 這就是你如何解決的。

1. 按一下您的名稱，然後選擇&#x200B;**Setup**。

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. 在左搜索欄中輸入&#x200B;**profile**，然後按一下&#x200B;**Manage Users**&#x200B;下的&#x200B;**Profiles**。

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. 按一下同步使用者的設定檔。

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. 在&#x200B;**欄位級安全性**&#x200B;區段下，按一下包含欄位的對象旁的&#x200B;**視圖**。

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. 按一下「**編輯**」。

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. 勾選您要新增至同步的欄位的&#x200B;**Visible**&#x200B;核取方塊，然後按一下&#x200B;**Save**。

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   真貼心！ 在下一個同步週期中，Marketo將看到該欄位並啟動魔術。

   >[!NOTE]
   >
   > 如果欄位在Salesforce中已有值，則這些值要等到下次記錄更新時才會同步至Marketo。
