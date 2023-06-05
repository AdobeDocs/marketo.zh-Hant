---
description: 連線到Outlook - Marketo檔案 — 產品檔案
title: 連線到Outlook
source-git-commit: 2538bd5973eb3372352c3ddbada6521911f9fc33
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 連線到Outlook {#connect-to-outlook}

瞭解如何將Sales Insight Actions帳戶與Outlook連結。

>[!NOTE]
>
>每位使用者都必須從其Marketo Sales帳戶連線至Outlook。

## 正在連線到Outlook Online {#connecting-to-outlook-online}

連線到Outlook表示您將會收到回覆追蹤、存取Outlook傳遞通道、在Outlook中排程電子郵件以及傳送規範的能力。

1. 在Marketo Sales中，按一下齒輪圖示並選取 **設定**.

   ![](assets/connect-to-outlook-1.png)

1. 在我的帳戶下，選取 **電子郵件設定**.

   ![](assets/connect-to-outlook-2.png)

1. 按一下 **電子郵件連線** 標籤。

   ![](assets/connect-to-outlook-3.png)

1. 按一下 **開始使用**.

   ![](assets/connect-to-outlook-4.png)

1. 選取 **我使用Outlook傳送電子郵件** 並按一下 **下一個**.

   ![](assets/connect-to-outlook-5.png)

1. 選取您正在使用的Outlook版本，然後按一下 **下一個**. 在此範例中，我們選擇Outlook Online。

   ![](assets/connect-to-outlook-6.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>也稱為Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-premise</strong></td> 
      <td>包括Exchange 2013和2016</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Marketo目前不支援Exchange混合式帳戶。

1. 按一下 **確定**.

   ![](assets/connect-to-outlook-7.png)

1. 如果您尚未登入Outlook，請輸入登入資訊並按一下 **下一個**. 如果是，請選擇您要連線的帳戶，然後按一下 **下一個**. 在此範例中，我們已登入。

   ![](assets/connect-to-outlook-8.png)

1. 按一下 **Accept**.

   ![](assets/connect-to-outlook-9.png)

   您可以使用此連線來追蹤電子郵件，也可以作為傳遞管道。

   >[!NOTE]
   >
   >Outlook Online (Office365)會強制執行自己的傳送限制。 [在此處瞭解更多](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## 正在連線到Exchange On-Premise {#connecting-to-exchange-on-premise}

連線到Exchange內部部署表示您將會收到回覆追蹤、存取Outlook傳遞管道、在Outlook中排程電子郵件以及傳送合規性的功能。

1. 在Marketo Sales中，按一下齒輪圖示並選取 **設定**.

   ![](assets/connect-to-outlook-10.png)

1. 在我的帳戶下，選取 **電子郵件設定**.

   ![](assets/connect-to-outlook-11.png)

1. 按一下 **電子郵件連線** 標籤。

   ![](assets/connect-to-outlook-12.png)

1. 按一下 **開始使用**.

   ![](assets/connect-to-outlook-13.png)

1. 選取 **我使用Outlook傳送電子郵件** 並按一下 **下一個**.

   ![](assets/connect-to-outlook-14.png)

1. 選取您正在使用的Outlook版本，然後按一下 **下一個**. 在此範例中，我們選擇Exchange On-premise。

   ![](assets/connect-to-outlook-15.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>也稱為Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-premise</strong></td> 
      <td>包括Exchange 2013和2016</td> 
     </tr>
    </tbody>
   </table>

1. 輸入您的認證，然後按一下 **Connect**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >如果您在Exchange版本下拉式清單中關閉自動探索，您必須向IT部門詢問Exchange URL。

   您可以使用此連線來追蹤電子郵件，也可以作為傳遞管道。

   >[!NOTE]
   >
   >使用Exchange內部部署時，您的IT團隊將建立您的電子郵件傳送限制。

## 正在取得連線至Outlook Online的許可權 {#getting-permission-to-connect-to-outlook-online}

您可能需要與IT團隊合作，才能取得Marketo Sales連線至您Outlook Online帳戶(Microsoft 365)的許可權。

>[!NOTE]
>
>通知管理您Microsoft 365帳戶的IT團隊，需要存取的應用程式為「Marketo Sales Connect」。

根據您IT團隊的偏好設定和目前的設定，最好諮詢他們如何授予存取許可權。 以下是一些有助於引導交談的文章。

* 全域同意： [適用於Microsoft 365管理員的整合式應用程式和Azure AD](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* 使用者同意： [設定使用者如何同意應用程式](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&amp;pivots=portal){target="_blank"}
* 管理員同意： [設定管理員同意工作流程](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* 開啟或關閉使用者同意： [在Microsoft 365中管理使用者對應用程式的同意](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* 使用Microsoft Defender進行管理： [管理OAuth應用程式](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
