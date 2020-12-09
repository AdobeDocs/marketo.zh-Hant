---
unique-page-id: 2953471
description: SFDC同步——自訂物件同步——行銷檔案——產品檔案
title: SFDC同步——自定義對象同步
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# SFDC同步：自訂物件同步 {#sfdc-sync-custom-object-sync}

在Salesforce例項中建立的自訂物件也可以是Marketo的一部分。  這是如何設定的。

>[!NOTE]
>
>**需要管理員權限**

>[!PREREQUISITES]
>
>要使用自定義對象，它必須與Salesforce中的 [Lead](sfdc-sync-lead-sync.md)、 [](sfdc-sync-contact-sync.md)Contector [](sfdc-sync-account-sync.md)帳戶對象關聯。

## 啟用自訂物件  {#enable-custom-object}

1. 按一 **下「管理** 」和** 「Salesforce物件同步 **」連結**。**

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. 如果這是您的第一個自訂物件，請按一下「同 **步結構」。**

   ![](assets/rtaimage-2.png)

1. 按一下 **停用全域同步。**

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce自訂物件架構的初始同步可能需要幾分鐘的時間。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 將您要同步的自訂物件拖曳至畫布中。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自訂物件必須有唯一的名稱。 Marketo不支援兩個名稱相同的不同自訂物件。

1. 按一下 **啟用同步。**

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 再次單 **擊「啟用同步** 」。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >別忘了重新啟用全域同步！

1. 返回**Salesforce **標籤。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 按一下 **啟用同步。**

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 若要檢視所有Salesforce自訂物件，請按一下「管 **理** 」和**「Salesforce物件同步」**連結（與上述步驟1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo僅支援連結至一或兩層深之標準實體的自訂實體。

### 下一步： {#whats-next}

[將自定義對象欄位添加／刪除為智慧清單／觸發器約束](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

太棒了！ 您現在可以在智慧型促銷活動和智慧型清單中使用此自訂物件的資料。

