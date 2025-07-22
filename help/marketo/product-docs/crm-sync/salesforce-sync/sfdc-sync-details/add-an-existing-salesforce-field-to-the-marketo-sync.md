---
unique-page-id: 4719308
description: 將現有的Salesforce欄位新增至Marketo同步 — Marketo檔案 — 產品檔案
title: 新增現有的Salesforce欄位至Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# 新增現有[!DNL Salesforce]欄位至Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理員許可權**

通常，Salesforce中的新自訂欄位會自動同步至Marketo Engage。 如果沒有，Marketo Sync使用者可能無法看見這些欄位。 以下說明修正方法。

1. 按一下您的名稱，然後選取&#x200B;**[!UICONTROL Setup]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 在左側搜尋列中輸入「設定檔」，然後按一下&#x200B;**[!UICONTROL Profiles]**&#x200B;下方的&#x200B;**[!UICONTROL Manage Users]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 按一下同步處理使用者的設定檔。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. 在&#x200B;**[!UICONTROL Field-Level Security]**&#x200B;區段下，按一下包含欄位之物件旁的&#x200B;**[!UICONTROL View]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 勾選您要新增至同步處理之欄位的&#x200B;**[!UICONTROL Visible]**&#x200B;核取方塊，然後按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   在下一個同步處理週期中，Marketo將會看見該欄位並開始施展魔術。

   >[!NOTE]
   >
   > 如果欄位在[!DNL Salesforce]中已有值，則這些值要等到下次記錄更新時才會同步至Marketo。
