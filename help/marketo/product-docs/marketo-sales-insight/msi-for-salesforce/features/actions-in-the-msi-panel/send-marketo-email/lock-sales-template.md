---
unique-page-id: 12981050
description: 鎖定銷售範本 — Marketo檔案 — 產品檔案
title: 鎖定銷售範本
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 4%

---

# 鎖定銷售範本 {#lock-sales-template}

為了防止CRM使用者編輯銷售範本，管理員可以啟用鎖定範本的功能，然後讓使用者可以從電子郵件編輯器個別鎖定範本。

>[!CAUTION]
>
>此功能僅適用於[!DNL Salesforce]，與[!DNL Microsoft Dynamics]或其他CRM不相容。 不會鎖定從[!DNL Outlook]或Gmail外掛程式存取的範本，因為編輯器不受Marketo控制。

## 啟用鎖定範本 {#enable-lock-template}

>[!NOTE]
>
>**需要管理員許可權**

1. 移至&#x200B;**[!UICONTROL Admin]**，然後按一下&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/1.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;底下，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/2.png)

1. 檢查&#x200B;**[!UICONTROL Enable ability to lock templates]**。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>預設會勾選此方塊，並啟用鎖定範本的功能。 取消核取此選項將停用電子郵件編輯器中的鎖定範本功能。

>[!NOTE]
>
>以管理員身分變更此設定&#x200B;**不會**&#x200B;回溯影響現有的範本；也就是說，它不會自動鎖定它們。

## 在電子郵件編輯器中鎖定範本 {#lock-template-in-the-email-editor}

1. 選取您要鎖定的電子郵件，然後按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/5.png)

1. 在電子郵件編輯器中，按一下&#x200B;**[!UICONTROL Email Settings]**。

   ![](assets/6.png)

1. 檢查&#x200B;**[!UICONTROL Publish to Marketo Sales Insight]** （如果尚未檢查）。 您現在可以取消核取&#x200B;**[!UICONTROL Allow CRM user to edit email]**&#x200B;以鎖定範本。 按一下「**[!UICONTROL Save]**」。

   ![](assets/7.png)

   >[!NOTE]
   >
   >預設會勾選此方塊，並允許CRM使用者編輯電子郵件。
