---
unique-page-id: 2953471
description: SFDC同步——自定義對象同步-Marketo文檔——產品文檔
title: SFDC同步——自定義對象同步
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# SFDC同步：自訂物件同步{#sfdc-sync-custom-object-sync}

在Salesforce例項中建立的自訂物件也可以是Marketo的一部分。  這是如何設定的。

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>若要使用自訂物件，它必須與Salesforce中的[lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)、[contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)或[account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)物件相關聯。

## 啟用自訂物件{#enable-custom-object}

1. 按一下「**管理員**」和「**Salesforce物件同步**」連結。

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. 如果這是您的第一個自定義對象，請按一下&#x200B;**同步方案**。

   ![](assets/rtaimage-2.png)

1. 按一下&#x200B;**禁用全局同步**。

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce自訂物件架構的初始同步可能需要幾分鐘的時間。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 將您要同步的自訂物件拖曳至畫布中。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自訂物件必須有唯一的名稱。 Marketo不支援兩個同名的不同自訂物件。

1. 按一下&#x200B;**啟用同步**。

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 再次按一下&#x200B;**啟用同步**。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >別忘了重新啟用全域同步！

1. 返回&#x200B;**Salesforce**&#x200B;標籤。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 按一下&#x200B;**啟用同步**。

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 若要檢視所有Salesforce自訂物件，請按一下&#x200B;**Admin**&#x200B;和&#x200B;**Salesforce物件同步**&#x200B;連結（與上述步驟1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至一或兩層深之標準實體的自訂實體。

### 下一步：{#whats-next}

[將自定義對象欄位添加／刪除為智慧清單／觸發器約束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

太棒了！ 您現在可以在智慧型促銷活動和智慧型清單中使用此自訂物件的資料。
