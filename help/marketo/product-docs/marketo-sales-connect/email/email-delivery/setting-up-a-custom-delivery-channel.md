---
unique-page-id: 14746470
description: 設定自訂傳遞管道 — Marketo檔案 — 產品檔案
title: 設定自訂傳遞通道
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 設定自訂傳遞通道 {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect可讓您整合自訂SMTP伺服器，以傳送您的電子郵件。 對於不想從Gmail或Exchange傳遞通道傳送大量電子郵件的使用者來說，這是一個絕佳選項。

使用者可以設定自訂SMTP伺服器以供其個人使用，或管理員可以設定Team SMTP供您執行個體中的所有Sales Connect使用者共用。

>[!NOTE]
>
>* 除了設定SMTP伺服器之外，您必須先驗證您的[電子郵件身分識別](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)，才能傳送電子郵件。
>* 建議您與您的IT團隊或SMTP伺服器供應商合作，取得SMTP伺服器的正確伺服器認證。
>* 您無法使用SMTP伺服器認證來連線您的Gmail和Exchange伺服器。 請使用我們的電子郵件連線服務來與這些提供者整合。

## 自訂SMTP {#custom-smtp}

1. 登入[網頁應用程式](https://toutapp.com/login)，按一下右上方的齒輪圖示，然後選擇&#x200B;**設定**。

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. 在「我的帳戶」底下，按一下&#x200B;**電子郵件設定**。

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. 按一下&#x200B;**自訂傳遞通道**。

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. 輸入您的SMTP伺服器認證，然後按一下&#x200B;**連線**。

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >如果這是您唯一的傳遞頻道，則會自動指派給您所有電子郵件身分識別，而您已在此完成。 如果這不是您唯一的傳遞管道，請繼續前往步驟5。

1. 當仍在電子郵件設定中時，按一下&#x200B;**地址和簽名**。

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. 尋找您要選擇傳遞管道的電子郵件身分識別，然後按一下&#x200B;**選擇傳遞管道**。

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. 在傳遞能力卡中，按一下&#x200B;**編輯**。

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. 按一下「頻道」下拉式清單，然後選擇您剛才新增的自訂傳送頻道。 按一下&#x200B;**保存**。

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >如果您的團隊管理員設定了Team SMTP Server，它只會自動套用至您的預設電子郵件身分識別，並且可作為您其他電子郵件身分識別的選項。

## Team SMTP伺服器 {#team-smtp-server}

>[!NOTE]
>
>**需要管理員許可權**

1. 登入[網頁應用程式](https://toutapp.com/login)，按一下右上方的齒輪圖示，然後選擇&#x200B;**設定**。

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. 在[管理設定]下，按一下[一般] **&#x200B;**。

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. 按一下&#x200B;**團隊傳遞管道**。

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. 輸入您的SMTP伺服器認證，然後按一下&#x200B;**連線**。

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Team SMTP Server將是所有團隊成員預設電子郵件身分的預設傳遞通道。 此外，它將成為所有其他電子郵件身分識別的傳送通道選項。

   >[!MORELIKETHIS]
   >
   >* Gmail使用者的[電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [電子郵件連線給Outlook使用者](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
