---
unique-page-id: 14746470
description: 設定自訂傳遞管道 — Marketo檔案 — 產品檔案
title: 設定自訂傳遞管道
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 4%

---

# 設定自訂傳遞管道 {#setting-up-a-custom-delivery-channel}

[!DNL Marketo Sales Connect]可讓您整合自訂SMTP伺服器，以傳遞您的電子郵件。 對於不想從Gmail或[!DNL Exchange]傳遞通道傳送大量電子郵件的使用者，這是一個很好的選項。

使用者可以設定自訂SMTP伺服器以供其個人使用，或管理員可以設定要在您執行個體中的所有[!DNL Sales Connect]使用者共用的團隊SMTP。

>[!NOTE]
>
>* 除了設定SMTP伺服器之外，您必須先驗證您的[電子郵件身分識別](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)，才能傳送電子郵件。
>* 建議您與您的IT團隊或SMTP伺服器供應商合作，取得SMTP伺服器的正確伺服器認證。
>* 您無法使用SMTP伺服器認證連線您的Gmail和[!DNL Exchange]伺服器。 請使用我們的電子郵件連線服務來與這些提供者整合。

## 自訂SMTP {#custom-smtp}

1. 登入[網頁應用程式](https://toutapp.com/login)，按一下右上方的齒輪圖示並選擇&#x200B;**[!UICONTROL Settings]**。

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. 在[!UICONTROL My Account]底下，按一下&#x200B;**[!UICONTROL Email Settings]**。

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. 按一下「**[!UICONTROL Custom Delivery Channel]**」。

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. 輸入您的[!UICONTROL SMTP Server]認證並按一下&#x200B;**[!UICONTROL Connect]**。

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >如果這是您唯一的傳遞頻道，則會自動指派給您所有電子郵件身分識別，而您已在此完成。 如果這不是您唯一的傳遞管道，請繼續前往步驟5。

1. 當仍在[!UICONTROL Email Settings]中時，按一下&#x200B;**[!UICONTROL Address and Signature]**。

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. 尋找您要選擇傳遞管道的電子郵件身分識別，然後按一下&#x200B;**[!UICONTROL Choose Delivery Channel]**。

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. 在[!UICONTROL Deliverability]卡片中，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. 按一下[!UICONTROL Channel]下拉式清單，然後選擇您剛才新增的自訂傳遞管道。 按一下「**[!UICONTROL Save]**」。

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >如果您的團隊管理員設定了Team SMTP Server，它只會自動套用至您的預設電子郵件身分識別，並且可作為您其他電子郵件身分識別的選項。

## Team SMTP伺服器 {#team-smtp-server}

>[!NOTE]
>
>**需要管理員許可權**

1. 登入[網頁應用程式](https://toutapp.com/login)，按一下右上方的齒輪圖示並選擇&#x200B;**[!UICONTROL Settings]**。

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**[!UICONTROL General]**。

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. 按一下「**[!UICONTROL Team Delivery Channel]**」。

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. 輸入您的[!UICONTROL SMTP Server]認證並按一下&#x200B;**[!UICONTROL Connect]**。

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Team SMTP Server將是所有團隊成員預設電子郵件身分的預設傳遞通道。 此外，它將成為所有其他電子郵件身分識別的傳送通道選項。

   >[!MORELIKETHIS]
   >
   >* Gmail使用者的[電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [位使用者的 [!DNL Outlook] 電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
