---
unique-page-id: 12981050
description: 鎖定銷售範本——行銷人員檔案——產品檔案
title: 鎖定銷售模板
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# 鎖定銷售模板{#lock-sales-template}

為防止CRM使用者編輯銷售範本，管理員可啟用鎖定範本的功能，如此可讓使用者從電子郵件編輯器中個別鎖定範本。

>[!CAUTION]
>
>此功能僅適用於Salesforce，且與Microsoft Dynamics或其他CRM不相容。 從Outlook或Gmail外掛程式存取的範本不會鎖定，因為編輯器不受Marketo控制。

## 啟用鎖定模板{#enable-lock-template}

>[!NOTE]
>
>**需要管理員權限**

1. 前往&#x200B;**Admin**，然後按一下&#x200B;**Sales Insight**。

   ![](assets/1.png)

1. 在&#x200B;**Settings**&#x200B;下，按一下&#x200B;**Edit**。

   ![](assets/2.png)

1. 檢查&#x200B;**啟用鎖定模板的功能**。 按一下&#x200B;**保存**。

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>預設情況下，此框處於選中狀態，並啟用了鎖定模板的功能。 取消勾選會停用電子郵件編輯器中的鎖定範本功能。

>[!NOTE]
>
>將此設定變更為管理員會對現有範本造成&#x200B;**not**&#x200B;回溯影響；即，它不會自動鎖住它們。

## 在電子郵件編輯器中鎖定模板{#lock-template-in-the-email-editor}

1. 選擇您要鎖定的電子郵件，然後按一下「編輯草稿」。****

   ![](assets/5.png)

1. 在電子郵件編輯器中，按一下&#x200B;**電子郵件設定**。

   ![](assets/6.png)

1. 如果尚未勾選，請勾選「發佈至Marketo Sales Insight **」。**&#x200B;您現在可以取消勾選「允許CRM使用者編輯電子郵件&#x200B;**」，以鎖定範本。**&#x200B;按一下&#x200B;**保存**。

   ![](assets/7.png)

   >[!NOTE]
   >
   >依預設，此方塊會勾選並允許CRM使用者編輯電子郵件。
