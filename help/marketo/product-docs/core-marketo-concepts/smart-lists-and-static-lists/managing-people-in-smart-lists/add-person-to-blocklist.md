---
unique-page-id: 9438139
description: 將人員新增至封鎖清單 — Marketo檔案 — 產品檔案
title: 將個人新增至封鎖清單
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 1%

---

# 將個人新增至封鎖清單 {#add-person-to-blocklist}

將人員新增至您的封鎖清單會防止他們收到您的信件。

1. 建立新的[預設程式](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"}，並將其命名為「加入封鎖清單」。

1. 按一下&#x200B;**[!UICONTROL New]**&#x200B;並選取&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/add-person-to-blocklist-1.png)

1. 選擇「**[!UICONTROL Smart List]**」。

   ![](assets/add-person-to-blocklist-2.png)

1. 為清單命名，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/add-person-to-blocklist-3.png)

1. 將所有人員新增至您的智慧清單中，以便將其新增至封鎖清單中。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >封鎖清單上的人員不會收到操作電子郵件。

1. 返回您的程式。

   ![](assets/add-person-to-blocklist-5.png)

1. 按一下&#x200B;**[!UICONTROL New]**&#x200B;並選取&#x200B;**[!UICONTROL New Smart Campaign]**。

   ![](assets/add-person-to-blocklist-6.png)

1. 為新的Smart Campaign命名。 按一下「**[!UICONTROL Create]**」。

   ![](assets/add-person-to-blocklist-7.png)

1. 拖放&#x200B;**[!UICONTROL Member of Smart List]**。

   ![](assets/add-person-to-blocklist-8.png)

1. 選取您剛建立的智慧清單。

   ![](assets/add-person-to-blocklist-9.png)

1. 按一下「**[!UICONTROL Flow]**」標籤。 拖放&#x200B;**[!UICONTROL Change Data Value]**&#x200B;流量動作。

   ![](assets/add-person-to-blocklist-10.png)

1. 在&#x200B;**[!UICONTROL Attribute]**&#x200B;下拉式清單中選取&#x200B;**[!UICONTROL Block Listed]**&#x200B;並將&#x200B;**[!UICONTROL New Value]**&#x200B;設為&#x200B;**[!UICONTROL true]**。

   ![](assets/add-person-to-blocklist-11.png)

1. 按一下「**[!UICONTROL Schedule]**」索引標籤並選取「**[!UICONTROL Run Once]**」。

   ![](assets/add-person-to-blocklist-12.png)

1. 選取&#x200B;**[!UICONTROL Run Now]**&#x200B;並按一下&#x200B;**[!UICONTROL Run]**。

   ![](assets/add-person-to-blocklist-13.png)

1. 再按一下&#x200B;**[!UICONTROL Run]**。

   ![](assets/add-person-to-blocklist-14.png)

這些人將不再收到電子郵件。

>[!TIP]
>
>使用[變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}建立&#x200B;**觸發行銷活動**，其中列出的&#x200B;**區塊為True**，適用於未來所有具有可列入封鎖清單屬性的人員。
