---
unique-page-id: 4719308
description: 將現有的Salesforce欄位新增至Marketo同步 — Marketo檔案 — 產品檔案
title: 將現有的Salesforce欄位新增至Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 81bc90bcccc8073511c9f331471c0cda9f4147cb
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 將現有的Salesforce欄位新增至Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理權限**

通常，Salesforce中的新自訂欄位會自動同步至Marketo。 否則，Marketo同步使用者可能看不到這些欄位。 這就是你如何解決的。

1. 按一下您的名稱，然後選取 **設定**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 輸入 **設定檔** 在左側搜尋列中，按一下 **設定檔** 在 **管理使用者**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 按一下同步使用者的設定檔。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. 在 **欄位層級安全性** ，按一下 **檢視** 在包含欄位的物件旁。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 按一下 **編輯**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 檢查 **可見** 要添加到同步的欄位的複選框，然後按一下 **儲存**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   真貼心！ 在下一個同步週期中，Marketo將看到該欄位並啟動魔術。

   >[!NOTE]
   >
   > 如果欄位在Salesforce中已有值，則這些值要等到下次記錄更新時才會同步至Marketo。
