---
unique-page-id: 9438139
description: 將人員新增至封鎖清單 — Marketo檔案 — 產品檔案
title: 將個人新增至封鎖清單
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# 將個人新增至封鎖清單 {#add-person-to-blocklist}

將人員新增至您的封鎖清單會防止他們收到您的信件。

1. [建立新的預設程式](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 並為其命名 **新增至封鎖清單**.

1. 按一下 **新增** 並選取 **新增本機資產**.

   ![](assets/add-person-to-blocklist-1.png)

1. 選取 **智慧清單**.

   ![](assets/add-person-to-blocklist-2.png)

1. 為清單命名，然後按一下 **建立**.

   ![](assets/add-person-to-blocklist-3.png)

1. 將所有人員新增至 **智慧清單** 您想要新增至封鎖清單中。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >封鎖清單上的人員不會收到操作電子郵件。

1. 返回您的程式。

   ![](assets/add-person-to-blocklist-5.png)

1. 按一下 **新增** 並選取 **新增智慧型行銷活動**.

   ![](assets/add-person-to-blocklist-6.png)

1. 為命名 **新增智慧型行銷活動**. 按一下 **建立**。

   ![](assets/add-person-to-blocklist-7.png)

1. 拖放 **智慧清單的成員**.

   ![](assets/add-person-to-blocklist-8.png)

1. 選取您剛建立的智慧清單。

   ![](assets/add-person-to-blocklist-9.png)

1. 按一下 **流量** 標籤。 拖放 **變更資料值** 流量動作。

   ![](assets/add-person-to-blocklist-10.png)

1. 在 **屬性** 下拉式清單選取 **區塊已列出** 並設定 **新值** 至 **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. 按一下 **排程** 標籤並選取 **執行一次**.

   ![](assets/add-person-to-blocklist-12.png)

1. 選取 **立即執行** 並按一下 **執行**.

   ![](assets/add-person-to-blocklist-13.png)

1. 按一下 **執行** 再來一次。

   ![](assets/add-person-to-blocklist-14.png)

這些人將不再收到電子郵件。

>[!TIP]
>
>建立 [觸發智慧行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) 使用 **變更資料值** 替換為 **封鎖清單為true** 適用於未來所有具有可封鎖清單屬性的人。
