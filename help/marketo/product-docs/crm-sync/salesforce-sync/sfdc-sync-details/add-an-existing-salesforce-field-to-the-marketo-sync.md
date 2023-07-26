---
unique-page-id: 4719308
description: 將現有Salesforce欄位新增至Marketo同步 — Marketo檔案 — 產品檔案
title: 將現有Salesforce欄位新增至Marketo同步
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 將現有Salesforce欄位新增至Marketo同步 {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**需要管理員許可權**

通常，Salesforce中的新自訂欄位會自動同步至Marketo。 如果沒有，Marketo Sync使用者可能無法看見這些欄位。 以下說明修正方法。

1. 按一下您的名稱，然後選取 **設定**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. 輸入 **設定檔** ，然後按一下 **設定檔** 在 **管理使用者**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. 按一下同步處理使用者的設定檔。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. 在 **欄位層級安全性** 區段，按一下 **檢視** 位於包含欄位的物件旁。

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. 按一下 **編輯**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. 檢查 **可見** 要新增至同步處理之欄位的核取方塊，然後按一下 **儲存**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   真貼心！ 在下一個同步處理週期中，Marketo將會看見該欄位並開始施展魔術。

   >[!NOTE]
   >
   > 如果欄位在Salesforce中已有值，則這些值要等到下次記錄更新時才會同步至Marketo。
